# DATA_SOURCES

## Primary dataset
Wu J, Zan X, Gao L, Zhao J, Fan J, Shi H, Wan Y, Yu E, Li S, Xie X.  
**A Machine Learning Method for Identifying Lung Cancer Based on Routine Blood Indices: Qualitative Feasibility Study.**  
*JMIR Medical Informatics* 2019;7(3):e13476. doi:10.2196/13476

- PubMed Central page (with supplementary files): https://pmc.ncbi.nlm.nih.gov/articles/PMC6714502/
- Download **Multimedia Appendix 1** (XLSX training and validation set) and **Multimedia Appendix 2** (XLSX test set) and place them in your local `data/` folder (this repo does not redistribute data).

## License
The article and its supplements are released under **CC BY 4.0**.  
When reusing, include attribution to the original authors and a link to the license.

## Reproduce locally
1. Download the XLSX from the PubMed Central page above.
2. Save to `data/`.
3. Open `notebooks/LC_RBT_end_to_end.ipynb` and run; outputs are written to `outputs/`.
