# Issue: Example Images Returning 404 in NextJS Frontend

## Symptoms
1. Example images (e.g. `/examples/complex/vl1_6_1.png`) in the frontend interface returned `404 Not Found`.
2. Inspecting the Nginx container logs revealed requests to `/examples/...` were being proxy-passed to the Next.js container (port 3000) which did not have these files in its public folder.

## Cause
The Nginx configuration template in `nginx.conf` and `scripts/admin_panel.py` only contained routing paths matching `/gradio_api/file=/app/...` (from the old Gradio UI version). Under the new Next.js frontend, example images are requested using the path `/examples/...`. Because Nginx lacked a location block for `/examples/`, it failed to intercept these requests and forwarded them to the Node backend instead.

## Solution
1. Added a location block for `/examples/` in `nginx.conf` pointing to `/usr/share/nginx/html/examples/`:
   ```nginx
   # Intercept requests for example images (NextJS path)
   location /examples/ {
       alias /usr/share/nginx/html/examples/;
       add_header Access-Control-Allow-Origin *;
   }
   ```
2. Updated the Nginx configuration template inside [scripts/admin_panel.py](../scripts/admin_panel.py) to preserve this routing behavior during dynamic GPU configuration updates.
3. Reloaded Nginx inside the container:
   ```bash
   docker compose exec nginx nginx -s reload
   ```
4. Example images now load correctly in the browser.
