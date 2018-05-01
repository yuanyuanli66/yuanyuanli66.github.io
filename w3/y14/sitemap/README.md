


## Research projects
1. Method for analyzing genome-wide protein binding patterns from ChIP-seq data
    * Proposed and implemented T-KDE toolbox, to identify the locations of constitutive protein binding sites using ChIP-seq data.
    * In contrast to existing bining or sliding windows approach, T-KDE combines a binary range tree with a kernel density estimator (KDE) to quickly identify constitutive protein binding sites from multiple cell lines. 
    * Kernel density estimation is a very expensive operation for human genome (3,234.83 Mega-basepairs per haploid genome
6,469.66 Mb total (diploid).). Using a binary tree to divide human chromosomes recurively into small regions allows KDE become an affordable operation. 
    * T-KDE can also identify genomic "hot spots" where several different proteins bind and, conversely, cell-specific sites from multiple cell lines. 

2. Nearest neighbor imputation in wireless sensor networks
    * Proposed and implemented KD-tree as nearest neighbor imputation method for wireless sensor networks
    * Proposed to use Mahalanobis distance for KD-tree construction instead of Euclidean distance
    * When impute for missing values in WSN, we not only consider sensors' past readings (temporal), but also nearby sensors' readings (spatial).   
    * The KD-tree NN imputation has similiar performances to state-of-the-art Expectation–Maximization (EM) missing data imputation but much faster.  


## Publications
* [Y. Li,  D. M. Umbach, and L. Li, "T-KDE: a method for genome-wide identification of constitutive protein binding sites from multiple ChIP-seq data sets", BMC genomics, Volume 15, Issue 1, Pages 27, January 2014.](https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-15-27)
**Abstract:**
*Background:* A protein may bind to its target DNA sites constitutively, i.e., regardless of cell type. Intuitively, constitutive binding sites should be biologically functional. A prerequisite for understanding their functional relevance is knowing all their locations for a protein of interest. Genome-wide discovery of constitutive binding sites requires robust and efficient computational methods to integrate results from numerous binding experiments. Such methods are lacking, however.
*Results:* To locate constitutive binding sites for a protein using ChIP-seq data for that protein from multiple cell lines, we developed a method, T-KDE, which combines a binary range tree with a kernel density estimator. Using 132 CTCF (CCCTC-binding factor) ChIP-seq datasets, we showed that the number of constitutive sites identified by T-KDE is robust to the choice of tuning parameter and that T-KDE identifies binding site locations more accurately than a binning approach. Furthermore, T-KDE can identify constitutive sites that are missed by a motif-based approach either because a bound site failed to reach the motif significance cutoff or because the peak sequence scanned was too short. By studying sites declared constitutive by T-KDE but not by the motif-based approach, we discovered two new CTCF motif variants. Using ENCODE data on 22 transcription factors (TF) in 132 cell lines, we identified constitutive binding sites for each TF and provide evidence that, for some TFs, they may be biologically meaningful.
*Conclusions:* T-KDE is an efficient and effective method to predict constitutive protein binding sites using ChIP-seq peaks from multiple cell lines. Besides constitutive binding sites for a given protein, T-KDE can identify genomic "hot spots" where several different proteins bind and, conversely, cell-type-specific sites bound by a given protein.



* [Y. Li and L. E. Parker, "Nearest neighbor imputation using spatial–temporal correlations in wireless sensor networks", Information Fusion, Volume 15, Pages 64-79, https://doi.org/10.1016/j.inffus.2012.08.007, Jan 2014.](https://www.sciencedirect.com/science/article/pii/S1566253512000711)
**Abstract:**
Missing data is common in Wireless Sensor Networks (WSNs), especially with multi-hop communications. There are many reasons for this phenomenon, such as unstable wireless communications, synchronization issues, and unreliable sensors. Unfortunately, missing data creates a number of problems for WSNs. First, since most sensor nodes in the network are battery-powered, it is too expensive to have the nodes re-transmit missing data across the network. Data re-transmission may also cause time delays when detecting abnormal changes in an environment. Furthermore, localized reasoning techniques on sensor nodes (such as machine learning algorithms to classify states of the environment) are generally not robust enough to handle missing data. Since sensor data collected by a WSN is generally correlated in time and space, we illustrate how replacing missing sensor values with spatially and temporally correlated sensor values can significantly improve the network’s performance. However, our studies show that it is important to determine which nodes are spatially and temporally correlated with each other. Simple techniques based on Euclidean distance are not sufficient for complex environmental deployments. Thus, we have developed a novel Nearest Neighbor (NN) imputation method that estimates missing data in WSNs by learning spatial and temporal correlations between sensor nodes. To improve the search time, we utilize a kd-tree data structure, which is a non-parametric, data-driven binary search tree. Instead of using traditional mean and variance of each dimension for kd-tree construction, and Euclidean distance for kd-tree search, we use weighted variances and weighted Euclidean distances based on measured percentages of missing data. We have evaluated this approach through experiments on sensor data from a volcano dataset collected by a network of Crossbow motes, as well as experiments using sensor data from a highway traffic monitoring application. Our experimental results show that our proposed -NN imputation method has a competitive accuracy with state-of-the-art Expectation–Maximization (EM) techniques, while using much simpler computational techniques, thus making it suitable for use in resource-constrained WSNs.

## Presentations

## Posters
A. Mateja 1, Y. Li, and L. Li, "Using T-KDE to Discover Novel Loci That May be Implicated in X-Inactivation", NIEHS Biostatistics Branch, summer internship program, poster presentation, 2014.

Affiliations: 1. The College of William and Mary

*Background:* In female mammals, one of the two X chromosomes is transcriptionally inactivated through a process called X chromosome inactivation.  This is because of dosage compensation between males, who only have one copy of the X chromosome, and females, who have two.  XIST is a gene that encodes a long, non-coding RNA that coats the inactive X chromosome and  is known to be one of the key players in this process.  Several other non-coding RNAs, such as TSIX and JPX, are also known to be involved in the X inactivation process.  The presence of the histone modifications h3k4me3 and h3k27ac in the promoter of XIST appear to be sex-specific in human cells.  This means that these marks are present in female cell lines, but not male cell lines. These markers are typically associated with activation of a particular gene; therefore, it follows that they should be seen near the promoter of XIST of all female cell lines (since XIST is expressed in every type of cell), but not male cell lines, since XIST is not expressed at all in males. 

*Objective:* Our objective was to find genes with similar patterns of histone markers as XIST using mouse cell lines, as these genes may also be involved in the X inactivation process. 

*Methods:* We downloaded narrow peak data for the h3k4me3 marker from 29 different cell lines, and data for the h3k27ac marker from 23 different cell lines from ENCODE.  This data was then run in T-KDE, a recently developed software that locates unique genomic loci with that mark in at least one of the data sets.  From there, we assigned a binary value of 0 to the cell line if the marker was not present, and 1 if it was.  The distinct pattern for the transcription start site of XIST was compared to other loci on the X-chromosome to see the percentage of cell line markings that they had in common.  Those with the highest correlation (>0.75) were analyzed to see what genes they corresponded to.  Any long non-coding RNAs were of particular interest.  

*Results:* We found several loci on the X chromosome that shared a high percentage of h3k4me3 markings with the TSS of XIST.  Several of these were located in or around the long non-coding RNA FIRRE, which is a homolog of the human LOC286467.  This locus was shown in humans to have a very similar histone pattern as the  XIST TSS.  In addition, there is a high correlation between the h3k4me3 and the h3k27ac patterns of the XIST TSS and that of 2010204K13Rik, another long coding RNA.  

*Conclusions:* Given the similarities the h3k4me3 patterns of the transcription start site of XIST with several loci within FIRRE, it is possible that FIRRE also plays a role in X inactivation, although further testing is needed to confirm.  In addition, given the similarities in both h3k4me3 and h3k27ac patterns between XIST and 2010204K13Rik, this locus could also be of interest in the process of X inactivation.


[presentation](../README.html)


