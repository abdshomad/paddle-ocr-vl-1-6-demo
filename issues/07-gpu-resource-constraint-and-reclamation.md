# Issue: vLLM Server Engine Core OOM on Startup due to Host GPU VRAM Constraints

## Symptoms
1. Running `docker compose up -d` started the services, but `vllm-server-gpu0-1` crashed repeatedly.
2. The logs of `vllm-server-gpu0-1` reported:
   `ValueError: Free memory on device (14.81/44.39 GiB) on startup is less than desired GPU memory utilization (0.5, 22.2 GiB). Decrease GPU memory utilization or reduce GPU memory used by other processes.`

## Cause
Other inactive/stale docker containers from other applications on the system (such as `ocr-arena-dotsocr-vllm-server`, `autolabel-backend`, and `slang-splat-demo-jul-2026-web-demo-1`) were running on GPU 0 and consuming ~15.3 GiB of VRAM. This left only ~14.8 GiB of free VRAM, which was less than the 22.2 GiB (50% of the 44.39 GiB L40 GPU) required by our vLLM server to start.

## Solution
1. Traced the container processes running on GPU 0 using `nvidia-smi` and matching container process PIDs to their container scopes:
   - `ocr-arena-dotsocr-vllm-server` (PID 1545467)
   - `autolabel-backend` (PID 1537625)
   - `slang-splat-demo-jul-2026-web-demo-1` (PID 1537708)
2. Stopped the conflicting, non-essential containers using:
   ```bash
   docker stop ocr-arena-dotsocr-vllm-server autolabel-backend slang-splat-demo-jul-2026-web-demo-1
   ```
3. Verified via `nvidia-smi` that VRAM usage on GPU 0 dropped significantly, leaving ~31.25 GiB of free VRAM.
4. Restarted the `vllm-server-gpu0` service:
   ```bash
   docker compose restart vllm-server-gpu0
   ```
5. This resolved the resource constraint, allowing the PyTorch model weights to load successfully without raising memory errors.
