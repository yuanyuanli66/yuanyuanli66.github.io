

## Research projects
1. Predict metastatic progression of melanoma using machine learning 
    * Predicted tumor progression and identified signature genes simultaneously using RNA-seq and miRNA-seq from The Cancer Genome Atlas (TCGA) melanoma (SKCM) data.
    * Challenges of the problem included: 1) large *P* small *N* (~20,000 genes x ~400 samples) and 2) perform gene selection and prediction at the same time.
    * Used Genetic Algorithm to select 20 genes at a time and used K-nearest neighbor to evaluate these genes' prediction performances (GA/KNN). 
    * Use GA to fully search the gene space is expansive, developed a parallelized version of GA using POSIX threads. 
    * Associated selected signature genes and miRNA with various clinical outcomes via statistical tests.
   
2. Pan-cancer analysis using TCGA RNA-seq data
    * Identified differential expressed genes that can predict 33 tumor types using GA/KNN multi-class classification.
    * The problem is challenging due to large data size (~20,000 genes x ~10,000 samples for 33 tumor types). 
    * It took ~ 1 month for GA/KNN to fully explore the solution space. 
    * Started exploring Gradient Boosted Machines (GBMs) as an alternative machine learning method for this problem. 
    * It only took GBMs a few hours to explore the solution space with higher classification accuracies.
    * Performed cluster analysis using signature genes.
    * Performed survival analysis (Cox regression model) using signature genes for all tumor types.



## Publications

* [Y. Li, K. Kang, J. M. Krahn, N. Croutwater, K. Lee, D. M. Umbach, and L. Li, "A comprehensive genomic pan-cancer classification using The Cancer Genome Atlas gene expression data", BMC genomics, Volume 18, Issue 1, Pages 508, July 2017.](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-017-3906-0)
**Abstract:**
*Background:* The Cancer Genome Atlas (TCGA) has generated comprehensive molecular profiles. We aim to identify a set of genes whose expression patterns can distinguish diverse tumor types. Those features may serve as biomarkers for tumor diagnosis and drug development.
*Methods:* Using RNA-seq expression data, we undertook a pan-cancer classification of 9,096 TCGA tumor samples representing 31 tumor types. We randomly assigned 75% of samples into training and 25% into testing, proportionally allocating samples from each tumor type.
*Results:* We could correctly classify more than 90% of the test set samples. Accuracies were high for all but three of the 31 tumor types, in particular, for READ (rectum adenocarcinoma) which was largely indistinguishable from COAD (colon adenocarcinoma). We also carried out pan-cancer classification, separately for males and females, on 23 sex non-specific tumor types (those unrelated to reproductive organs). Results from these gender-specific analyses largely recapitulated results when gender was ignored. Remarkably, more than 80% of the 100 most discriminative genes selected from each gender separately overlapped. Genes that were differentially expressed between genders included BNC1, FAT2, FOXA1, and HOXA11. FOXA1 has been shown to play a role for sexual dimorphism in liver cancer. The differentially discriminative genes we identified might be important for the gender differences in tumor incidence and survival.
*Conclusions:* We were able to identify many sets of 20 genes that could correctly classify more than 90% of the samples from 31 different tumor types using TCGA RNA-seq data. This accuracy is remarkable given the number of the tumor types and the total number of samples involved. We achieved similar results when we analyzed 23 non-sex-specific tumor types separately for males and females. We regard the frequency with which a gene appeared in those sets as measuring its importance for tumor classification. One third of the 50 most frequently appearing genes were pseudogenes; the degree of enrichment may be indicative of their importance in tumor classification. Lastly, we identified a few genes that might play a role in sexual dimorphism in certain cancers.


* [Y. Li, D. M. Umbach, and L. Li, "Putative genomic characteristics of BRAF V600K versus V600E cutaneous melanoma", Melanoma Research, Volume 27, Issue 6, Pages 527–535, December 2017.](https://journals.lww.com/melanomaresearch/Abstract/2017/12000/Putative_genomic_characteristics_of_BRAF_V600K.1.aspx)
**Abstract:**
Approximately 50% of all cutaneous melanomas harbor activating BRAF V600 mutations; among, these 10–30% carry the V600K mutation. Clinically, patients with V600K tumors experience distant metastases sooner and have an increased risk of relapse and shorter survival than patients with V600E tumors. Despite the clinical and other histopathological differences between these BRAF tumor subtypes, little is known about them at the genomic level. Herein, we systematically compared BRAF V600E and V600K skin cutaneous melanoma (SKCM) samples from the Cancer Genome Atlas (TCGA) for differential protein, gene, and microRNA expression genome-wide using the Mann–Whitney U-test. Our analyses showed that elements of energy-metabolism and protein-translation pathways were upregulated and that proapoptotic pathways were downregulated in V600K tumors compared with V600E tumors. We found that c-Kit protein and KIT gene expressions were significantly higher in V600K tumors than in V600E tumors, concurrent with significant downregulation of several KIT-targeting microRNAs (mir) including mir-222 in V600K tumors, suggesting KIT and mir-222 might be key genomic contributors toward the clinical differences observed. The relationship that we uncovered among KIT/c-Kit expression, mir-222 expression, and growth and prosurvival signals in V600 tumors is intriguing. We believe that the observed clinical aggressiveness of V600K tumors compared to V600E tumors may be attributable to the increased energy metabolism, protein translation and prosurvival signals compared with V600E tumors. If confirmed using larger numbers of V600K tumors, our results may prove useful for designing clinical management and targeted chemotherapeutical interventions for BRAF V600K-positive melanomas. Finally, the small sample size in V600K tumors is a major limitation of our study.



## Presentations

## Posters
* Y. Li, D. M. Umbach, L Li, "A comprehensive genomic pan-cancer analysis comparing males and females using The Cancer Genome Atlas gene expression data", AACR: Clinical Cancer Research 23, A46-A46, 2017.
**Abstract:**
The Cancer Genome Atlas (TCGA) has made available comprehensive molecular profiles including gene expression using RNA-seq for many human tumor types and, thereby, provided a great opportunity to use pan-cancer gene expression patterns to identify unique features that can classify tumor types. Those features may serve as biomarkers for tumor diagnosis and potential targets for drug development. Because gender differences in cancer susceptibility are one of the most consistent findings in cancer epidemiology, knowing whether the distinguishing features differ between males and females for the same tumor types might enhance their utility as biomarkers.

Our goals are: 1) to identify a set of genes whose expression levels can classify pan-cancer tumor types when gender is ignored; and 2) to identify analogous sets of genes for pan-cancer classification in sex non-specific tumors from men and from women separately.

Here we analyzed the RNA-seq expression data for 9,096 TCGA tumor samples from 31 tumor types; we selected features for sample classification using a genetic algorithm, GA/KNN, which we developed. We randomly assigned half of all samples into a training set and half into a test set, proportionally allocating samples from each tumor type. We used the training set to obtain 2,000 near-optimal classifiers (each set consisting of 20 genes) from repeated GA/KNN runs. We subsequently applied each resultant near-optimal classifier to the test set. The predicted class was then compared with the true class to calculate both training- and testing-set prediction accuracies. To see if sex non-specific tumors (those that are not related to reproductive organs) differ between males and females, we repeated the analysis for 24 sex non-specific tumor types separately for males and for females.

In the analysis ignoring gender, we could accurately classify 88.7% training samples and 88.1% of the testing samples on average. The top 20 genes that separated the 31 tumor types were TCF21, TBX5, EMX20S, EMX2, PA2G4P4, HNF1B, NACA2, SFTPA1, ATP5EP2, PTTG3P, FTHL3, ANXA2P3, GATA3, NAPSA, SFTA3, HSPB1P1, HOXA9, IGBP1P1, RPL19P12, and SFTPB.

Not surprisingly, we achieved similar average classification accuracies for testing samples (88.2% for males and 88.4% for females). Seventy four of the 100 top-ranked genes were common between males and females. The main reasons for less than total overlap between males and females are: stochastic nature of the algorithm, training/testing partitioning (only done once) and some intrinsic differences between genders. For example, BNC1, FAT2, and MSX2 ranked 36, 84, and 94 in males but 461, 603, and 1085 in females. Conversely, HPN, POU3F3, and FOXA1 ranked 75, 78, and 91 but 421, 355, and 349, respectively. It remains unclear whether genes likes those play any role in differential cancer susceptibility between genders.

In conclusion, we were able to select many sets of 20 genes that can correctly classify ~88% of the tumor samples from 31 different types for a validation set using RNA-seq gene expression alone. This accuracy is remarkable given the number of the tumor types involved. This result was largely replicated in tumors between genders. We were also identified a few genes that might play a role in gender differences among sex non-specific tumors.

[presentation](../README.html)


