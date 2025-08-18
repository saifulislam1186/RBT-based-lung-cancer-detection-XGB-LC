## Data source

This project uses the public dataset from:

Wu J, Zan X, Gao L, Zhao J, Fan J, Shi H, Wan Y, Yu E, Li S, Xie X.  
**A Machine Learning Method for Identifying Lung Cancer Based on Routine Blood Indices: Qualitative Feasibility Study.**  
*JMIR Medical Informatics* 2019;7(3):e13476. https://doi.org/10.2196/13476

The article (and its supplementary files) are available via PubMed Central.  
**License:** Creative Commons Attribution 4.0 (CC BY 4.0).  
© The authors. *“This is an open-access article distributed under the terms of the Creative Commons Attribution License (https://creativecommons.org/licenses/by/4.0/), which permits unrestricted use, distribution, and reproduction in any medium, provided the original work is properly cited.”* :contentReference[oaicite:2]{index=2}

We do not redistribute the raw data in this repository. See `DATA_SOURCES.md` for instructions to download from the original source.

## Environment
- Python: **3.10** (tested)
- Install deps: `pip install -r requirements.txt`

## Models included
- Logistic Regression, SVM (RBF/linear), Random Forest, Naive Bayes, AdaBoost
- Gradient boosting: XGBoost, LightGBM

## How to reproduce
1. Clone: `git clone https://github.com/saifulislam1186/RBT-based-lung-cancer-detection-XGB-LC.git`
2. `pip install -r requirements.txt`
3. Place CSVs in `data/` (not committed).
4. Open `notebooks/LC_RBT_end_to_end.ipynb` and run top-to-bottom.
5. Results are written to `outputs/` (metrics CSVs, tables,Excel).
