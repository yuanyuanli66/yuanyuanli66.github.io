


## Research projects
1. Method for analyzing genome-wide protein binding patterns from ChIP-seq data
    * Proposed and implemented T-KDE toolbox, to identify the locations of constitutive protein binding sites using ChIP-seq data.
    * T-KDE, which combines a binary range tree with a kernel density estimator (KDE) to quickly identify constitutive protein binding sites from multiple cell lines. 
    * T-KDE can also identify genomic "hot spots" where several different proteins bind and, conversely, cell-specific sites from multiple cell lines. 

2. Nearest neighbor imputation in wireless sensor networks
    * Proposed and implemented KD-tree as nearest neighbor imputation method for wireless sensor networks
    * Proposed to use Mahalanobis distance for KD-tree construction instead of Euclidean distance
    * When impute for missing values in WSN, we not only consider sensors' own past readings (temporal), but also nearby sensors' readings (spatial).   


## Publications
* [Y. Li,  D. M. Umbach, and L. Li, "T-KDE: a method for genome-wide identification of constitutive protein binding sites from multiple ChIP-seq data sets", BMC genomics, Volume 15, Issue 1, Pages 27, Jan 2013.](https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-15-27)
**Abstract:**
*Background:* A protein may bind to its target DNA sites constitutively, i.e., regardless of cell type. Intuitively, constitutive binding sites should be biologically functional. A prerequisite for understanding their functional relevance is knowing all their locations for a protein of interest. Genome-wide discovery of constitutive binding sites requires robust and efficient computational methods to integrate results from numerous binding experiments. Such methods are lacking, however.
*Results:* To locate constitutive binding sites for a protein using ChIP-seq data for that protein from multiple cell lines, we developed a method, T-KDE, which combines a binary range tree with a kernel density estimator. Using 132 CTCF (CCCTC-binding factor) ChIP-seq datasets, we showed that the number of constitutive sites identified by T-KDE is robust to the choice of tuning parameter and that T-KDE identifies binding site locations more accurately than a binning approach. Furthermore, T-KDE can identify constitutive sites that are missed by a motif-based approach either because a bound site failed to reach the motif significance cutoff or because the peak sequence scanned was too short. By studying sites declared constitutive by T-KDE but not by the motif-based approach, we discovered two new CTCF motif variants. Using ENCODE data on 22 transcription factors (TF) in 132 cell lines, we identified constitutive binding sites for each TF and provide evidence that, for some TFs, they may be biologically meaningful.
*Conclusions:* T-KDE is an efficient and effective method to predict constitutive protein binding sites using ChIP-seq peaks from multiple cell lines. Besides constitutive binding sites for a given protein, T-KDE can identify genomic "hot spots" where several different proteins bind and, conversely, cell-type-specific sites bound by a given protein.



* [Y. Li and L. E. Parker, "Nearest neighbor imputation using spatial–temporal correlations in wireless sensor networks", Information Fusion, Volume 15, Pages 64-79, https://doi.org/10.1016/j.inffus.2012.08.007, Jan 2014.](https://www.sciencedirect.com/science/article/pii/S1566253512000711)
**Abstract:**
Missing data is common in Wireless Sensor Networks (WSNs), especially with multi-hop communications. There are many reasons for this phenomenon, such as unstable wireless communications, synchronization issues, and unreliable sensors. Unfortunately, missing data creates a number of problems for WSNs. First, since most sensor nodes in the network are battery-powered, it is too expensive to have the nodes re-transmit missing data across the network. Data re-transmission may also cause time delays when detecting abnormal changes in an environment. Furthermore, localized reasoning techniques on sensor nodes (such as machine learning algorithms to classify states of the environment) are generally not robust enough to handle missing data. Since sensor data collected by a WSN is generally correlated in time and space, we illustrate how replacing missing sensor values with spatially and temporally correlated sensor values can significantly improve the network’s performance. However, our studies show that it is important to determine which nodes are spatially and temporally correlated with each other. Simple techniques based on Euclidean distance are not sufficient for complex environmental deployments. Thus, we have developed a novel Nearest Neighbor (NN) imputation method that estimates missing data in WSNs by learning spatial and temporal correlations between sensor nodes. To improve the search time, we utilize a kd-tree data structure, which is a non-parametric, data-driven binary search tree. Instead of using traditional mean and variance of each dimension for kd-tree construction, and Euclidean distance for kd-tree search, we use weighted variances and weighted Euclidean distances based on measured percentages of missing data. We have evaluated this approach through experiments on sensor data from a volcano dataset collected by a network of Crossbow motes, as well as experiments using sensor data from a highway traffic monitoring application. Our experimental results show that our proposed -NN imputation method has a competitive accuracy with state-of-the-art Expectation–Maximization (EM) techniques, while using much simpler computational techniques, thus making it suitable for use in resource-constrained WSNs.

## Presentations

[presentation](../README.html)


