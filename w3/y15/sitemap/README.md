


## Research projects
1. Predict metastatic progression of melanoma using machine learning 
    * Predicted tumor progression and identified signature genes simultaneously using RNA-seq and miRNA-seq from The Cancer Genome Atlas (TCGA) melanoma (SKCM) data.
    * Challenges of the problem included: 1) large *P* small *N* (~20,000 genes x ~400 samples) and 2) perform gene selection and prediction at the same time.
    * Used Genetic Algorithm to select 20 genes at a time and used K-nearest neighbor to evaluate these genes' prediction performances (GA/KNN). 
    * Use GA to fully search the gene space is expansive, developed a parallelized version of GA using POSIX threads. 
    * Associated selected signature genes and miRNA with various clinical outcomes via statistical tests.



## Publications
* [Y. Li, J. M. Krahn, G. P. Flake, D. M. Umbach, and L. Li, "Toward predicting metastatic progression of melanoma based on gene expression data", Pigment Cell & Melanoma Research, Volume 28, Issue 4, Pages 453-463, July 2015.](https://onlinelibrary.wiley.com/doi/full/10.1111/pcmr.12374)
**Abstract:**
Primary and metastatic melanoma tumors share the same cell origin, making it challenging to identify genomic biomarkers that can differentiate them. Primary tumors themselves can be heterogeneous, reflecting ongoing genomic changes as they progress toward metastasizing. We developed a computational method to explore this heterogeneity and to predict metastatic progression of the primary tumors. We applied our method separately to gene expression and to microRNA (miRNA) expression data from ~450 primary and metastatic skin cutaneous melanoma (SKCM) samples from the Cancer Genome Atlas (TCGA). Metastatic progression scores from RNA‐seq data were significantly associated with clinical staging of patients’ lymph nodes, whereas scores from miRNA‐seq data were significantly associated with Clark's level. The loss of expression of many characteristic epithelial lineage genes in primary SKCM tumor samples was highly correlated with predicted progression scores. We suggest that those genes/miRNAs might serve as putative biomarkers for SKCM metastatic progression. 


## Presentations

[presentation](../README.html)


