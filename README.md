# XGB-LC — Lung Cancer Detection from Routine Blood Tests

End-to-end, notebook-first pipeline to train, tune, feature-select, validate, threshold-optimize,
and test ML models (incl. **XGBoost & LightGBM**) for lung cancer detection using routine blood indices.  
Outputs are written to `outputs/`; the frozen model + metadata to `models/`.

---

## TL;DR Results (external test, fixed threshold 0.70)

| Model  | Accuracy % | Sensitivity | Specificity | Precision | AUC |
|--------|-----------:|------------:|------------:|----------:|----:|
| XGB-LC | **xx.x**   | **0.xxx**   | **0.xxx**   | **0.xxx** | **0.xxx** |

> After running the notebook, see `outputs/test_metrics_XGB-LC.csv`.

---

## How to run

### Option A — Conda
```bash
conda env create -f environment.yml
conda activate xgb-lc
python -m notebook

### Option B — pip + venv
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
python -m notebook

Then open notebooks/LC_RBT_end_to_end.ipynb and Run All.
If data/ is empty, a file picker lets you choose train/test files from anywhere on your PC.

## Data source

This project uses the public dataset from:

Wu J, Zan X, Gao L, Zhao J, Fan J, Shi H, Wan Y, Yu E, Li S, Xie X.
A Machine Learning Method for Identifying Lung Cancer Based on Routine Blood Indices: Qualitative Feasibility Study.
JMIR Medical Informatics 2019;7(3):e13476. https://doi.org/10.2196/13476

The article (and its supplementary files) are available via PubMed Central.
License: Creative Commons Attribution 4.0 (CC BY 4.0).
© The authors. “This is an open-access article distributed under the terms of the Creative Commons Attribution License (https://creativecommons.org/licenses/by/4.0/), which permits unrestricted use, distribution, and reproduction in any medium, provided the original work is properly cited.”

We do not redistribute the raw data in this repository. See DATA_SOURCES.md for instructions to download from the original source.

## Models included

Logistic Regression

SVM (RBF/linear)

Random Forest

Naive Bayes

AdaBoost

Gradient boosting: XGBoost, LightGBM

## Reproducibility

Python 3.10 (see environment.yml)

Seeds set in the notebook

Notebook outputs auto-stripped on commit (via nbstripout)

##License

Code released under the MIT License (see LICENSE).
No datasets are redistributed; see DATA_SOURCES.md.
