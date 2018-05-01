


## Research projects
1. Pan-cancer analysis using TCGA RNA-seq data
    * Identified differential expressed genes that can predict 33 tumor types using GA/KNN multi-class classification.
    * The problem is challenging due to large data size (~20,000 genes X ~10,000 samples for 33 tumor types). 
    * It took ~1 month for GA/KNN to fully explore the solution space. 
    * Started exploring Gradient Boosted Machines (GBMs) as an alternative machine learning method for this problem. 
    * It only took GBMs a few hours to explore the solution space with higher classification accuracies.
    * Performed cluster analysis using signature genes.
    * Performed survival analysis (Cox regression model) using signature genes for all tumor types.


## Posters
* [Y. Li, J. M. Krahn, N. Croutwater, K. Lee, D. M. Umbach, and L. Li, "A comprehensive genomic pan-cancer analysis using The Cancer Genome Atlas gene expression data"](../PanCancer_BSC_review_2016_v2.pdf)

* Yuanyuan Li, David M. Umbach, and Leping Li, "A comprehensive genomic pan-cancer analysis using The Cancer Genome Atlas gene expression data", FARE 2017, NIH, March 2016.
**Abstract:**
The Cancer Genome Atlas (TCGA) has made available comprehensive molecular profiles including gene expression for many human tumor types and provided a great opportunity to use those data to identify features that can classify tumor types. Because gender differences in cancer susceptibility are one of the most consistent findings in cancer epidemiology, knowing whether the distinguishing features differ between males and females for the same tumor types might enhance their utility as biomarkers.
Our goals are: to identify a set of genes whose expression levels can classify pan-cancer tumor types when gender is ignored; and to identify analogous sets of genes in sex non-specific tumors from men and from women separately.        
We analyzed RNA-seq data for 9096 TCGA tumor samples from 31 types using the GA/KNN algorithm we developed. We randomly assigned half of all samples into a training set and half into a test set, proportionally allocating samples from each tumor type and used the training set to obtain 2000 near-optimal classifiers (each set consisting of 20 genes) from repeated runs. We subsequently applied each resultant near-optimal classifier to the test set and compared the predicted class with the true class to calculate training and testing performances. To see if sex non-specific tumors (not related to reproductive organs) differ between males and females, we repeated the analysis for 24 tumor types separately for males and for females.
In all analyses, we could accurately classify ~89% training and ~88% testing samples. The top 20 genes that separated the 31 tumor types were TCF21, TBX5, EMX20S, EMX2, PA2G4P4, HNF1B, NACA2, SFTPA1, ATP5EP2, PTTG3P, FTHL3, ANXA2P3, GATA3, NAPSA, SFTA3, HSPB1P1, HOXA9, IGBP1P1, RPL19P12, and SFTPB.  
Of the 100 top-ranked genes, 74 were common between males and females. A few genes showed considerable difference in ranking between genders. For example, BNC1 ranked 36 in males but 461 in females. Literature showed that BNC1 was hypermethylated in female compared to male hepatocellular carcinoma. It remains unclear if the top genes played any role in differential cancer susceptibility between genders.
In conclusion, we were able to accurately classify ~88% of the tumor samples in all analyses. The performances are remarkable given the number of the tumor types (24 and 31) involved. We were also identified a few genes that might play a role in gender differences among sex non-specific tumors. 

 


## Presentations
* [Y. Li, "A comprehensive genomic pan-cancer classification using The Cancer Genome Atlas gene expression data", Biostatistics and Computational Biology Branch Retreat, 2016](../Pan-cancerClassification_yuanyuanli_BSC_review_2016.pdf)


