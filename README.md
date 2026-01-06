# Enhancing Cross-Patient Generalization in AI-Based Parkinson’s Disease Detection

This repository contains the **final experimental notebooks** used to reproduce the results reported in the paper:

**Enhancing Cross-Patient Generalization in AI-Based Parkinson’s Disease Detection**

The work focuses on improving Parkinson’s Disease (PD) detection from hand-drawn images by enhancing **generalization to unseen patients** using a drawing-aware, chunk-based approach.

---

## 📄 Paper Overview

Parkinson’s Disease affects fine motor control, which can be observed in drawing tasks such as **circles, meanders, and spirals**.  
While many prior works report high accuracy, they often suffer from **data leakage** due to image-wise evaluation, resulting in overly optimistic performance.

This work addresses that issue by:
- Enforcing **subject-wise evaluation**
- Using **2×2 image chunking** to capture localized motor irregularities
- Applying a **two-stage pipeline**:
  1. Drawing-type classification
  2. Parkinson’s Disease detection

The proposed method achieves strong and stable performance across **image-wise**, **subject-wise**, and **leave-one-subject-out** evaluations.

---

## 📁 Notebooks Included

The repository contains **three final notebooks**, each corresponding to a specific evaluation protocol used in the paper:

- **`Final_Solution_Image_wise.ipynb`**  
  Reproduces the **image-wise cross-validation (CV5)** results.

- **`Final_Solution_SubjectWise.ipynb`**  
  Reproduces the **subject-wise cross-validation (CV5)** results.

- **`Final_Solution_SubjectWise_LOO.ipynb`**  
  Reproduces the **Leave-One-Individual-Out (LOIO)** evaluation results.

Each notebook is **self-contained** and follows the same execution logic.

---

## 📊 Dataset

The experiments use the **NewHandPD** dataset, a publicly available Parkinson’s Disease handwriting dataset.

The dataset includes hand-drawn:
- Circles
- Meanders
- Spirals  

from both Parkinson’s patients and healthy controls.

> **Note:**  
> The dataset is **not included** in this repository and must be downloaded separately.

---

## 🚀 How to Reproduce the Results

### ✅ Required Step (Only One)

To recreate the results reported in the paper:

1. Open **any of the final solution notebooks**
2. Replace the dataset path with **your local dataset path**
3. Run the notebook

### Example:
```python
DATA_ROOT = "/your/path/to/NewHandPD"
