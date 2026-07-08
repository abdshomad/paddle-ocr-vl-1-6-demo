# PaddleOCR VL 1.6 Online Demo - Complete Test Results

This document presents the complete set of visual test results for both **Dark Mode** and **Light Mode** across all document categories, processing steps, and targeted element options.

## 1. General Application Flow & Authentication

These steps verify the initialization of Nginx reverse proxy, middleware redirection, and general app dashboard loading.

### Step 1: Sign-in Interface Redirection
![Sign-in Page](../screenshots/01-01-signin-page.jpg)

### Step 2: Main Dashboard Loaded
![Main Dashboard](../screenshots/02-02-main-page-loaded.jpg)

### Step 3: Default Layout Parser (Content Tab)
![Content Tab](../screenshots/03-03-ocr-completed.jpg)

### Step 4: Default Layout Parser (Visualization Tab)
![Visualization Tab](../screenshots/03-04-ocr-visualization.jpg)

## 2. Dark Mode Test Results

### 2.1 Complex Document Parsing
Verifies layout segmentation, document unwarping, and VLM extraction on complex multi-column or multi-page formats.

#### Case 01
- **Step 1: Document Processing / Unwarping**
  ![01_step1_vl1_6_1_processing.png](../screenshots/dark-mode/complex/01_step1_vl1_6_1_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![01_step2_vl1_6_1_result.png](../screenshots/dark-mode/complex/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Document Processing / Unwarping**
  ![02_step1_vl1_6_10_processing.png](../screenshots/dark-mode/complex/02_step1_vl1_6_10_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![02_step2_vl1_6_10_result.png](../screenshots/dark-mode/complex/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Document Processing / Unwarping**
  ![03_step1_vl1_6_11_processing.png](../screenshots/dark-mode/complex/03_step1_vl1_6_11_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![03_step2_vl1_6_11_result.png](../screenshots/dark-mode/complex/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Document Processing / Unwarping**
  ![04_step1_vl1_6_12_processing.png](../screenshots/dark-mode/complex/04_step1_vl1_6_12_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![04_step2_vl1_6_12_result.png](../screenshots/dark-mode/complex/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Document Processing / Unwarping**
  ![05_step1_vl1_6_2_processing.png](../screenshots/dark-mode/complex/05_step1_vl1_6_2_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![05_step2_vl1_6_2_result.png](../screenshots/dark-mode/complex/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Document Processing / Unwarping**
  ![06_step1_vl1_6_3_processing.png](../screenshots/dark-mode/complex/06_step1_vl1_6_3_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![06_step2_vl1_6_3_result.png](../screenshots/dark-mode/complex/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Document Processing / Unwarping**
  ![07_step1_vl1_6_4_processing.png](../screenshots/dark-mode/complex/07_step1_vl1_6_4_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![07_step2_vl1_6_4_result.png](../screenshots/dark-mode/complex/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Document Processing / Unwarping**
  ![08_step1_vl1_6_5_processing.png](../screenshots/dark-mode/complex/08_step1_vl1_6_5_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![08_step2_vl1_6_5_result.png](../screenshots/dark-mode/complex/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Document Processing / Unwarping**
  ![09_step1_vl1_6_6_processing.png](../screenshots/dark-mode/complex/09_step1_vl1_6_6_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![09_step2_vl1_6_6_result.png](../screenshots/dark-mode/complex/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Document Processing / Unwarping**
  ![10_step1_vl1_6_7_processing.png](../screenshots/dark-mode/complex/10_step1_vl1_6_7_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![10_step2_vl1_6_7_result.png](../screenshots/dark-mode/complex/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Document Processing / Unwarping**
  ![11_step1_vl1_6_8_processing.png](../screenshots/dark-mode/complex/11_step1_vl1_6_8_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![11_step2_vl1_6_8_result.png](../screenshots/dark-mode/complex/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Document Processing / Unwarping**
  ![12_step1_vl1_6_9_processing.png](../screenshots/dark-mode/complex/12_step1_vl1_6_9_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![12_step2_vl1_6_9_result.png](../screenshots/dark-mode/complex/12_step2_vl1_6_9_result.png)

### 2.2 Targeted Element Recognition
Validates extraction of specific elements (e.g. running formulas, tabular layouts, or signature regions).

#### Case 01
- **Step 1: Processing Elements**
  ![01_step1_vl1_6_1_processing.png](../screenshots/dark-mode/targeted/01_step1_vl1_6_1_processing.png)

- **Step 2: Element Extraction Result**
  ![01_step2_vl1_6_1_result.png](../screenshots/dark-mode/targeted/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Processing Elements**
  ![02_step1_vl1_6_10_processing.png](../screenshots/dark-mode/targeted/02_step1_vl1_6_10_processing.png)

- **Step 2: Element Extraction Result**
  ![02_step2_vl1_6_10_result.png](../screenshots/dark-mode/targeted/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Processing Elements**
  ![03_step1_vl1_6_11_processing.png](../screenshots/dark-mode/targeted/03_step1_vl1_6_11_processing.png)

- **Step 2: Element Extraction Result**
  ![03_step2_vl1_6_11_result.png](../screenshots/dark-mode/targeted/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Processing Elements**
  ![04_step1_vl1_6_12_processing.png](../screenshots/dark-mode/targeted/04_step1_vl1_6_12_processing.png)

- **Step 2: Element Extraction Result**
  ![04_step2_vl1_6_12_result.png](../screenshots/dark-mode/targeted/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Processing Elements**
  ![05_step1_vl1_6_2_processing.png](../screenshots/dark-mode/targeted/05_step1_vl1_6_2_processing.png)

- **Step 2: Element Extraction Result**
  ![05_step2_vl1_6_2_result.png](../screenshots/dark-mode/targeted/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Processing Elements**
  ![06_step1_vl1_6_3_processing.png](../screenshots/dark-mode/targeted/06_step1_vl1_6_3_processing.png)

- **Step 2: Element Extraction Result**
  ![06_step2_vl1_6_3_result.png](../screenshots/dark-mode/targeted/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Processing Elements**
  ![07_step1_vl1_6_4_processing.png](../screenshots/dark-mode/targeted/07_step1_vl1_6_4_processing.png)

- **Step 2: Element Extraction Result**
  ![07_step2_vl1_6_4_result.png](../screenshots/dark-mode/targeted/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Processing Elements**
  ![08_step1_vl1_6_5_processing.png](../screenshots/dark-mode/targeted/08_step1_vl1_6_5_processing.png)

- **Step 2: Element Extraction Result**
  ![08_step2_vl1_6_5_result.png](../screenshots/dark-mode/targeted/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Processing Elements**
  ![09_step1_vl1_6_6_processing.png](../screenshots/dark-mode/targeted/09_step1_vl1_6_6_processing.png)

- **Step 2: Element Extraction Result**
  ![09_step2_vl1_6_6_result.png](../screenshots/dark-mode/targeted/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Processing Elements**
  ![10_step1_vl1_6_7_processing.png](../screenshots/dark-mode/targeted/10_step1_vl1_6_7_processing.png)

- **Step 2: Element Extraction Result**
  ![10_step2_vl1_6_7_result.png](../screenshots/dark-mode/targeted/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Processing Elements**
  ![11_step1_vl1_6_8_processing.png](../screenshots/dark-mode/targeted/11_step1_vl1_6_8_processing.png)

- **Step 2: Element Extraction Result**
  ![11_step2_vl1_6_8_result.png](../screenshots/dark-mode/targeted/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Processing Elements**
  ![12_step1_vl1_6_9_processing.png](../screenshots/dark-mode/targeted/12_step1_vl1_6_9_processing.png)

- **Step 2: Element Extraction Result**
  ![12_step2_vl1_6_9_result.png](../screenshots/dark-mode/targeted/12_step2_vl1_6_9_result.png)

### 2.3 Spotting & Seal Recognition
Specifically tests identification of stamps, signatures, official seals, and key signature fields.

#### Case 01
- **Step 1: Detecting Stamps & Seals**
  ![01_step1_vl1_6_1_processing.png](../screenshots/dark-mode/spotting/01_step1_vl1_6_1_processing.png)

- **Step 2: Stamps & Seals Output**
  ![01_step2_vl1_6_1_result.png](../screenshots/dark-mode/spotting/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Detecting Stamps & Seals**
  ![02_step1_vl1_6_10_processing.png](../screenshots/dark-mode/spotting/02_step1_vl1_6_10_processing.png)

- **Step 2: Stamps & Seals Output**
  ![02_step2_vl1_6_10_result.png](../screenshots/dark-mode/spotting/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Detecting Stamps & Seals**
  ![03_step1_vl1_6_11_processing.png](../screenshots/dark-mode/spotting/03_step1_vl1_6_11_processing.png)

- **Step 2: Stamps & Seals Output**
  ![03_step2_vl1_6_11_result.png](../screenshots/dark-mode/spotting/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Detecting Stamps & Seals**
  ![04_step1_vl1_6_12_processing.png](../screenshots/dark-mode/spotting/04_step1_vl1_6_12_processing.png)

- **Step 2: Stamps & Seals Output**
  ![04_step2_vl1_6_12_result.png](../screenshots/dark-mode/spotting/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Detecting Stamps & Seals**
  ![05_step1_vl1_6_2_processing.png](../screenshots/dark-mode/spotting/05_step1_vl1_6_2_processing.png)

- **Step 2: Stamps & Seals Output**
  ![05_step2_vl1_6_2_result.png](../screenshots/dark-mode/spotting/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Detecting Stamps & Seals**
  ![06_step1_vl1_6_3_processing.png](../screenshots/dark-mode/spotting/06_step1_vl1_6_3_processing.png)

- **Step 2: Stamps & Seals Output**
  ![06_step2_vl1_6_3_result.png](../screenshots/dark-mode/spotting/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Detecting Stamps & Seals**
  ![07_step1_vl1_6_4_processing.png](../screenshots/dark-mode/spotting/07_step1_vl1_6_4_processing.png)

- **Step 2: Stamps & Seals Output**
  ![07_step2_vl1_6_4_result.png](../screenshots/dark-mode/spotting/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Detecting Stamps & Seals**
  ![08_step1_vl1_6_5_processing.png](../screenshots/dark-mode/spotting/08_step1_vl1_6_5_processing.png)

- **Step 2: Stamps & Seals Output**
  ![08_step2_vl1_6_5_result.png](../screenshots/dark-mode/spotting/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Detecting Stamps & Seals**
  ![09_step1_vl1_6_6_processing.png](../screenshots/dark-mode/spotting/09_step1_vl1_6_6_processing.png)

- **Step 2: Stamps & Seals Output**
  ![09_step2_vl1_6_6_result.png](../screenshots/dark-mode/spotting/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Detecting Stamps & Seals**
  ![10_step1_vl1_6_7_processing.png](../screenshots/dark-mode/spotting/10_step1_vl1_6_7_processing.png)

- **Step 2: Stamps & Seals Output**
  ![10_step2_vl1_6_7_result.png](../screenshots/dark-mode/spotting/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Detecting Stamps & Seals**
  ![11_step1_vl1_6_8_processing.png](../screenshots/dark-mode/spotting/11_step1_vl1_6_8_processing.png)

- **Step 2: Stamps & Seals Output**
  ![11_step2_vl1_6_8_result.png](../screenshots/dark-mode/spotting/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Detecting Stamps & Seals**
  ![12_step1_vl1_6_9_processing.png](../screenshots/dark-mode/spotting/12_step1_vl1_6_9_processing.png)

- **Step 2: Stamps & Seals Output**
  ![12_step2_vl1_6_9_result.png](../screenshots/dark-mode/spotting/12_step2_vl1_6_9_result.png)

## 3. Light Mode Test Results

### 3.1 Complex Document Parsing
Verifies layout segmentation and OCR extraction in Light Mode.

#### Case 01
- **Step 1: Document Processing / Unwarping**
  ![01_step1_vl1_6_1_processing.png](../screenshots/light-mode/complex/01_step1_vl1_6_1_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![01_step2_vl1_6_1_result.png](../screenshots/light-mode/complex/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Document Processing / Unwarping**
  ![02_step1_vl1_6_10_processing.png](../screenshots/light-mode/complex/02_step1_vl1_6_10_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![02_step2_vl1_6_10_result.png](../screenshots/light-mode/complex/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Document Processing / Unwarping**
  ![03_step1_vl1_6_11_processing.png](../screenshots/light-mode/complex/03_step1_vl1_6_11_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![03_step2_vl1_6_11_result.png](../screenshots/light-mode/complex/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Document Processing / Unwarping**
  ![04_step1_vl1_6_12_processing.png](../screenshots/light-mode/complex/04_step1_vl1_6_12_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![04_step2_vl1_6_12_result.png](../screenshots/light-mode/complex/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Document Processing / Unwarping**
  ![05_step1_vl1_6_2_processing.png](../screenshots/light-mode/complex/05_step1_vl1_6_2_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![05_step2_vl1_6_2_result.png](../screenshots/light-mode/complex/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Document Processing / Unwarping**
  ![06_step1_vl1_6_3_processing.png](../screenshots/light-mode/complex/06_step1_vl1_6_3_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![06_step2_vl1_6_3_result.png](../screenshots/light-mode/complex/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Document Processing / Unwarping**
  ![07_step1_vl1_6_4_processing.png](../screenshots/light-mode/complex/07_step1_vl1_6_4_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![07_step2_vl1_6_4_result.png](../screenshots/light-mode/complex/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Document Processing / Unwarping**
  ![08_step1_vl1_6_5_processing.png](../screenshots/light-mode/complex/08_step1_vl1_6_5_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![08_step2_vl1_6_5_result.png](../screenshots/light-mode/complex/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Document Processing / Unwarping**
  ![09_step1_vl1_6_6_processing.png](../screenshots/light-mode/complex/09_step1_vl1_6_6_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![09_step2_vl1_6_6_result.png](../screenshots/light-mode/complex/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Document Processing / Unwarping**
  ![10_step1_vl1_6_7_processing.png](../screenshots/light-mode/complex/10_step1_vl1_6_7_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![10_step2_vl1_6_7_result.png](../screenshots/light-mode/complex/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Document Processing / Unwarping**
  ![11_step1_vl1_6_8_processing.png](../screenshots/light-mode/complex/11_step1_vl1_6_8_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![11_step2_vl1_6_8_result.png](../screenshots/light-mode/complex/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Document Processing / Unwarping**
  ![12_step1_vl1_6_9_processing.png](../screenshots/light-mode/complex/12_step1_vl1_6_9_processing.png)

- **Step 2: Parsing Layout & OCR Text Extraction**
  ![12_step2_vl1_6_9_result.png](../screenshots/light-mode/complex/12_step2_vl1_6_9_result.png)

### 3.2 Targeted Element Recognition
Validates extraction of specific elements in Light Mode.

#### Case 01
- **Step 1: Processing Elements**
  ![01_step1_vl1_6_1_processing.png](../screenshots/light-mode/targeted/01_step1_vl1_6_1_processing.png)

- **Step 2: Element Extraction Result**
  ![01_step2_vl1_6_1_result.png](../screenshots/light-mode/targeted/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Processing Elements**
  ![02_step1_vl1_6_10_processing.png](../screenshots/light-mode/targeted/02_step1_vl1_6_10_processing.png)

- **Step 2: Element Extraction Result**
  ![02_step2_vl1_6_10_result.png](../screenshots/light-mode/targeted/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Processing Elements**
  ![03_step1_vl1_6_11_processing.png](../screenshots/light-mode/targeted/03_step1_vl1_6_11_processing.png)

- **Step 2: Element Extraction Result**
  ![03_step2_vl1_6_11_result.png](../screenshots/light-mode/targeted/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Processing Elements**
  ![04_step1_vl1_6_12_processing.png](../screenshots/light-mode/targeted/04_step1_vl1_6_12_processing.png)

- **Step 2: Element Extraction Result**
  ![04_step2_vl1_6_12_result.png](../screenshots/light-mode/targeted/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Processing Elements**
  ![05_step1_vl1_6_2_processing.png](../screenshots/light-mode/targeted/05_step1_vl1_6_2_processing.png)

- **Step 2: Element Extraction Result**
  ![05_step2_vl1_6_2_result.png](../screenshots/light-mode/targeted/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Processing Elements**
  ![06_step1_vl1_6_3_processing.png](../screenshots/light-mode/targeted/06_step1_vl1_6_3_processing.png)

- **Step 2: Element Extraction Result**
  ![06_step2_vl1_6_3_result.png](../screenshots/light-mode/targeted/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Processing Elements**
  ![07_step1_vl1_6_4_processing.png](../screenshots/light-mode/targeted/07_step1_vl1_6_4_processing.png)

- **Step 2: Element Extraction Result**
  ![07_step2_vl1_6_4_result.png](../screenshots/light-mode/targeted/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Processing Elements**
  ![08_step1_vl1_6_5_processing.png](../screenshots/light-mode/targeted/08_step1_vl1_6_5_processing.png)

- **Step 2: Element Extraction Result**
  ![08_step2_vl1_6_5_result.png](../screenshots/light-mode/targeted/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Processing Elements**
  ![09_step1_vl1_6_6_processing.png](../screenshots/light-mode/targeted/09_step1_vl1_6_6_processing.png)

- **Step 2: Element Extraction Result**
  ![09_step2_vl1_6_6_result.png](../screenshots/light-mode/targeted/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Processing Elements**
  ![10_step1_vl1_6_7_processing.png](../screenshots/light-mode/targeted/10_step1_vl1_6_7_processing.png)

- **Step 2: Element Extraction Result**
  ![10_step2_vl1_6_7_result.png](../screenshots/light-mode/targeted/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Processing Elements**
  ![11_step1_vl1_6_8_processing.png](../screenshots/light-mode/targeted/11_step1_vl1_6_8_processing.png)

- **Step 2: Element Extraction Result**
  ![11_step2_vl1_6_8_result.png](../screenshots/light-mode/targeted/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Processing Elements**
  ![12_step1_vl1_6_9_processing.png](../screenshots/light-mode/targeted/12_step1_vl1_6_9_processing.png)

- **Step 2: Element Extraction Result**
  ![12_step2_vl1_6_9_result.png](../screenshots/light-mode/targeted/12_step2_vl1_6_9_result.png)

### 3.3 Targeted Element Types (Sub-variants)
Checks distinct element parser classes (Chart, Formula, Seal, Table, Text) dynamically.

#### Chart Recognition
- **Step 1: Processing Elements**
  ![01_step1_chart_recognition_processing.png](../screenshots/light-mode/targeted_element_types/01_step1_chart_recognition_processing.png)

- **Step 2: Final Parser Output**
  ![01_step2_chart_recognition_result.png](../screenshots/light-mode/targeted_element_types/01_step2_chart_recognition_result.png)

#### Formula Recognition
- **Step 1: Processing Elements**
  ![01_step1_formula_recognition_processing.png](../screenshots/light-mode/targeted_element_types/01_step1_formula_recognition_processing.png)

- **Step 2: Final Parser Output**
  ![01_step2_formula_recognition_result.png](../screenshots/light-mode/targeted_element_types/01_step2_formula_recognition_result.png)

#### Seal Recognition
- **Step 1: Processing Elements**
  ![01_step1_seal_recognition_processing.png](../screenshots/light-mode/targeted_element_types/01_step1_seal_recognition_processing.png)

- **Step 2: Final Parser Output**
  ![01_step2_seal_recognition_result.png](../screenshots/light-mode/targeted_element_types/01_step2_seal_recognition_result.png)

#### Table Recognition
- **Step 1: Processing Elements**
  ![01_step1_table_recognition_processing.png](../screenshots/light-mode/targeted_element_types/01_step1_table_recognition_processing.png)

- **Step 2: Final Parser Output**
  ![01_step2_table_recognition_result.png](../screenshots/light-mode/targeted_element_types/01_step2_table_recognition_result.png)

#### Text Recognition
- **Step 1: Processing Elements**
  ![01_step1_text_recognition_processing.png](../screenshots/light-mode/targeted_element_types/01_step1_text_recognition_processing.png)

- **Step 2: Final Parser Output**
  ![01_step2_text_recognition_result.png](../screenshots/light-mode/targeted_element_types/01_step2_text_recognition_result.png)

### 3.4 Spotting & Seal Recognition
Specifically tests stamp, seal, and signature detection under Light Mode styling.

#### Case 01
- **Step 1: Detecting Stamps & Seals**
  ![01_step1_vl1_6_1_processing.png](../screenshots/light-mode/spotting/01_step1_vl1_6_1_processing.png)

- **Step 2: Stamps & Seals Output**
  ![01_step2_vl1_6_1_result.png](../screenshots/light-mode/spotting/01_step2_vl1_6_1_result.png)

#### Case 02
- **Step 1: Detecting Stamps & Seals**
  ![02_step1_vl1_6_10_processing.png](../screenshots/light-mode/spotting/02_step1_vl1_6_10_processing.png)

- **Step 2: Stamps & Seals Output**
  ![02_step2_vl1_6_10_result.png](../screenshots/light-mode/spotting/02_step2_vl1_6_10_result.png)

#### Case 03
- **Step 1: Detecting Stamps & Seals**
  ![03_step1_vl1_6_11_processing.png](../screenshots/light-mode/spotting/03_step1_vl1_6_11_processing.png)

- **Step 2: Stamps & Seals Output**
  ![03_step2_vl1_6_11_result.png](../screenshots/light-mode/spotting/03_step2_vl1_6_11_result.png)

#### Case 04
- **Step 1: Detecting Stamps & Seals**
  ![04_step1_vl1_6_12_processing.png](../screenshots/light-mode/spotting/04_step1_vl1_6_12_processing.png)

- **Step 2: Stamps & Seals Output**
  ![04_step2_vl1_6_12_result.png](../screenshots/light-mode/spotting/04_step2_vl1_6_12_result.png)

#### Case 05
- **Step 1: Detecting Stamps & Seals**
  ![05_step1_vl1_6_2_processing.png](../screenshots/light-mode/spotting/05_step1_vl1_6_2_processing.png)

- **Step 2: Stamps & Seals Output**
  ![05_step2_vl1_6_2_result.png](../screenshots/light-mode/spotting/05_step2_vl1_6_2_result.png)

#### Case 06
- **Step 1: Detecting Stamps & Seals**
  ![06_step1_vl1_6_3_processing.png](../screenshots/light-mode/spotting/06_step1_vl1_6_3_processing.png)

- **Step 2: Stamps & Seals Output**
  ![06_step2_vl1_6_3_result.png](../screenshots/light-mode/spotting/06_step2_vl1_6_3_result.png)

#### Case 07
- **Step 1: Detecting Stamps & Seals**
  ![07_step1_vl1_6_4_processing.png](../screenshots/light-mode/spotting/07_step1_vl1_6_4_processing.png)

- **Step 2: Stamps & Seals Output**
  ![07_step2_vl1_6_4_result.png](../screenshots/light-mode/spotting/07_step2_vl1_6_4_result.png)

#### Case 08
- **Step 1: Detecting Stamps & Seals**
  ![08_step1_vl1_6_5_processing.png](../screenshots/light-mode/spotting/08_step1_vl1_6_5_processing.png)

- **Step 2: Stamps & Seals Output**
  ![08_step2_vl1_6_5_result.png](../screenshots/light-mode/spotting/08_step2_vl1_6_5_result.png)

#### Case 09
- **Step 1: Detecting Stamps & Seals**
  ![09_step1_vl1_6_6_processing.png](../screenshots/light-mode/spotting/09_step1_vl1_6_6_processing.png)

- **Step 2: Stamps & Seals Output**
  ![09_step2_vl1_6_6_result.png](../screenshots/light-mode/spotting/09_step2_vl1_6_6_result.png)

#### Case 10
- **Step 1: Detecting Stamps & Seals**
  ![10_step1_vl1_6_7_processing.png](../screenshots/light-mode/spotting/10_step1_vl1_6_7_processing.png)

- **Step 2: Stamps & Seals Output**
  ![10_step2_vl1_6_7_result.png](../screenshots/light-mode/spotting/10_step2_vl1_6_7_result.png)

#### Case 11
- **Step 1: Detecting Stamps & Seals**
  ![11_step1_vl1_6_8_processing.png](../screenshots/light-mode/spotting/11_step1_vl1_6_8_processing.png)

- **Step 2: Stamps & Seals Output**
  ![11_step2_vl1_6_8_result.png](../screenshots/light-mode/spotting/11_step2_vl1_6_8_result.png)

#### Case 12
- **Step 1: Detecting Stamps & Seals**
  ![12_step1_vl1_6_9_processing.png](../screenshots/light-mode/spotting/12_step1_vl1_6_9_processing.png)

- **Step 2: Stamps & Seals Output**
  ![12_step2_vl1_6_9_result.png](../screenshots/light-mode/spotting/12_step2_vl1_6_9_result.png)

