# Issue: Docker Network Subnet Exhaustion on Startup

## Symptoms
1. Running `docker compose up -d` failed with:
   `failed to create network paddle-ocr-vl-1-6-demo_default: Error response from daemon: all predefined address pools have been fully subnetted`

## Cause
The host system had 33 active or stale Docker bridge networks from various development demos. Docker's default subnet allocator exhausted all predefined IP pools, preventing it from creating the new default bridge network (`paddle-ocr-vl-1-6-demo_default`) required for our services to communicate.

## Solution
1. Inspected the existing networks using `docker network ls`.
2. Cleaned up stale, unused Docker networks by running:
   ```bash
   docker network prune -f
   ```
3. This successfully deleted several inactive bridge networks, freeing up subnet pools.
4. Reran `docker compose up -d`, which successfully created the default network and started all 20 containers.
