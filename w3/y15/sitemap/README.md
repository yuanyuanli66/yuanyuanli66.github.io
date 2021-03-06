


## Research projects
1. Predict metastatic progression of melanoma using machine learning 
    * Predicted tumor progression and identified signature genes simultaneously using RNA-seq and miRNA-seq from The Cancer Genome Atlas (TCGA) melanoma (SKCM) data.
    * Challenges of the problem included: 1) large *P* small *N* (~20,000 genes X ~400 samples) and 2) perform gene selection and prediction at the same time.
    * Used Genetic Algorithm to select 20 genes at a time and used K-nearest neighbor to evaluate these genes' prediction performances (GA/KNN). 
    * Use GA to fully search the gene space is expansive, developed a parallelized version of GA using POSIX threads. 
    * Associated selected signature genes and miRNA with various clinical outcomes via statistical tests.



## Publications
* [Y. Li, J. M. Krahn, G. P. Flake, D. M. Umbach, and L. Li, "Toward predicting metastatic progression of melanoma based on gene expression data", Pigment Cell & Melanoma Research, Volume 28, Issue 4, Pages 453-463, July 2015.](https://onlinelibrary.wiley.com/doi/full/10.1111/pcmr.12374)
**Abstract:**
Primary and metastatic melanoma tumors share the same cell origin, making it challenging to identify genomic biomarkers that can differentiate them. Primary tumors themselves can be heterogeneous, reflecting ongoing genomic changes as they progress toward metastasizing. We developed a computational method to explore this heterogeneity and to predict metastatic progression of the primary tumors. We applied our method separately to gene expression and to microRNA (miRNA) expression data from ~450 primary and metastatic skin cutaneous melanoma (SKCM) samples from the Cancer Genome Atlas (TCGA). Metastatic progression scores from RNA‐seq data were significantly associated with clinical staging of patients’ lymph nodes, whereas scores from miRNA‐seq data were significantly associated with Clark's level. The loss of expression of many characteristic epithelial lineage genes in primary SKCM tumor samples was highly correlated with predicted progression scores. We suggest that those genes/miRNAs might serve as putative biomarkers for SKCM metastatic progression. 


## Presentations
* [Y. Li, "TCGA PanCancer Analysis: feature interaction", group report, 2015.](../FeatureInteraction.pdf)


## Posters
* [C. R. Weinberg, M. Shi, A. Wise, D. M. Umbach, J. Krahn, Y. Li, L. Li, "A Stochastic Search Algorithm for Finding Multi-SNP Effects Using Nuclear Families", 2015.](../restructuredIGES2015_Sept29-v2_dmucrw.pdf)

* Y. Li, J. M. Krahn, G. P. Flake, D. M. Umbach, and L. Li, "Towards predicting metastatic progression of skin cutaneous melanoma based on gene expression data", FARE 2016, NIH, March 2015. 
**Abstract:**
Primary and metastatic melanoma tumors share the same cell origin, making it challenging to identify genomic biomarkers that can differentiate them. Primary tumors themselves can also be heterogeneous, reflecting ongoing genomic changes as they progress toward metastasizing. We developed a computational method to explore this heterogeneity and to predict metastatic progression of the primary tumors using the metastatic samples as a reference point. We applied our method separately to gene expression and to microRNA (miRNA) expression data from ~450 primary and metastatic skin cutaneous melanoma (SKCM) samples from the Cancer Genome Atlas (TCGA). Our analysis identified many gene/miRNA signatures that can largely distinguish primary from metastatic SKCM tumors. Furthermore, we uncovered that loss of expression of many characteristic epithelial lineage genes such as KRT17, S100A7, S100A7A, and mir-205 in primary SKCM tumor samples is highly correlated with predicted metastatic progression scores of those tumors. The metastatic progression scores obtained from RNA-seq data were significantly associated with patients’ clinical staging of their lymph nodes whereas the scores obtained from miRNA-seq data were significantly associated with Clark’s level. We suggest that those genes/miRNAs might serve as putative biomarkers for SKCM metastatic progression. Our unique approach is promising step toward allowing clinicians to assess the likelihood of metastatic progression of primary melanoma based on gene expression measurements.


