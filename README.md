
# Hybrid-GWAS-Modeling

Comparative modeling of SNP selection and phenotype prediction using sparse linear models (L₀-regularization) and non-linear models (Random Forests) on the QTLMAS 2010 GWAS dataset.

---

## Overview
This project investigates and compares sparse linear and non-linear modeling strategies to identify significant SNPs associated with a quantitative trait in GWAS data. The objective is to benchmark model sparsity, generalization, and biological interpretability in high-dimensional genomic data.

## Objectives
- Apply and evaluate **L₀-regularized regression** and **Random Forest** models for SNP selection and phenotype prediction.
- Explore hybrid modeling workflows combining sparse feature selection with non-linear model ranking.
- Analyze the biological relevance of selected SNPs and their mapped genes.

---

## Methods
- **Dataset:** QTLMAS 2010 GWAS dataset (3,226 individuals, 9,723 SNPs).
- **Approaches:**
  - **L₀-Regularization:** Iterative Hard Thresholding (IHT), Greedy Forward Selection, L0Learn R package (via Python `rpy2`).
  - **Random Forest:** Hyperparameter tuning, importance filtering, cumulative feature selection.
- **Tools & Libraries:** Python, R, L0Learn, Scikit-learn, Random Forest, Iterative Hard Thresholding, Pandas, Seaborn, Matplotlib.

---

## Key Results
- **L₀-regularized models:** Achieved **>85% SNP selection stability**, identified **<80 SNPs**, and reduced **Test MSE to 0.77**.
- **Random Forest:** Overfitted on the dataset (Test R² ≈ 0.30), revealing the additive nature of the trait with few dominant SNPs.
- **Biological Findings:** Key SNPs mapped to genes like **PRKAB2, RHOA, and SPTBN1**, linked to metabolic and neuronal pathways.

---

## Contributors
This was a collaborative project by:
- Sanyukta Chapagain ([LinkedIn](https://linkedin.com/in/sanyukta-chapagain))  
- Divyansh Rana  
- Vinamrata Sharma  
- Pranay Bandaru  
- Virija Nandamudi  

---

## Acknowledgments
We would like to thank our mentors and peers for their guidance and support throughout this project.  


---

## License
This project is shared for academic and learning purposes.  


