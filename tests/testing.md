# PaddleOCR VL 1.6 Online Demo - Testing Documentation

This document outlines the step-by-step testing procedure, automation logic, and visual results for verifying the containerized PaddleOCR VL 1.6 Online Demo application.

---

## 1. Automated Test Setup

The application features a Playwright browser automation script located at [scratch/test_ocr_demo.py](./scratch/test_ocr_demo.py) which performs end-to-end integration and visual regression testing:

*   **Framework**: Playwright (Python sync API)
*   **Target URL**: `http://localhost:7872` (Fronted by Nginx Proxy)
*   **Viewport**: 1280 x 1024 (Desktop)
*   **Browser**: Headless Chromium (with `--no-sandbox` and `--disable-dev-shm-usage` flags)

---

## 2. Test Steps & Verification

### Step 1: Navigating to the Login Screen
*   **Action**: Browser navigates to `http://localhost:7872`.
*   **Behavior**: Next.js auth middleware intercepts the unauthenticated session and redirects the request to `/signin`.
*   **Verification**: Wait for `input[placeholder="Enter your username"]` to render.
*   **Screenshot**: `01-01-signin-page.jpg`
*   **Visual Output**:
    ![Sign-in Page](../screenshots/01-01-signin-page.jpg)

### Step 2: Authentication
*   **Action**: Input username `demo`, input password `demo`, and click the "Sign In" button.
*   **Behavior**: API endpoint `/api/auth` authenticates the credentials, sets the `session_token` HTTP-only cookie, and redirects the browser back to `/` (home dashboard).
*   **Verification**: Wait for page URL redirection to resolve to the root, and ensure the example images sidebar gallery is loaded (wait for `img[src*='/examples/']`).
*   **Screenshot**: `02-02-main-page-loaded.jpg`
*   **Visual Output**:
    ![Main Dashboard Loaded](../screenshots/02-02-main-page-loaded.jpg)

### Step 3: Triggering Layout Parsing & OCR
*   **Action**: Select the first example card (`/examples/complex/vl1_6_1.png`) by clicking it.
*   **Behavior**: The UI triggers the layout parsing and OCR analysis request (`POST /api/parse`) with the selected example path, causing:
    1.  The UI to display an indeterminate loading progress bar.
    2.  `paddle-ocr-demo` container to route the parsing query to Nginx.
    3.  Nginx to proxy-pass to `pipeline-api-gpu0`.
    4.  `pipeline-api-gpu0` to process orientation (PP-LCNet), unwarping (UVDoc), and forward recognition requests to `vllm-server-gpu0`.
*   **Verification**: Wait for the loading progress indicator element (`.animate-fluent-progress`) to be removed/detached from the DOM (max timeout 60 seconds).
*   **Screenshot**: `03-03-ocr-completed.jpg`
*   **Visual Output (Text Extraction)**:
    ![OCR Completed (Content Tab)](../screenshots/03-03-ocr-completed.jpg)

### Step 4: Verification of Layout Visualization
*   **Action**: Click the "Visualization" (or "Visualisasi") tab header.
*   **Behavior**: The UI switches to show the unwarped layout image with bounding boxes drawn over detected sections (paragraphs, tables, titles, formulas).
*   **Verification**: Wait for the canvas elements to finish rendering.
*   **Screenshot**: `03-04-ocr-visualization.jpg`
*   **Visual Output (Visual Layout)**:
    ![OCR Bounding Box Visualization](../screenshots/03-04-ocr-visualization.jpg)

---

## 3. How to Run the Automated Test Suite

If you need to re-execute the test suite manually, make sure the docker containers are active and run:

```bash
# Activate the main python environment
source .venv/bin/activate

# Execute the playwright runner
python scratch/test_ocr_demo.py
```

All screenshots will be written directly to the [screenshots/](../screenshots/) folder.
