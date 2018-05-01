


## Research projects

1. Wireless sensor network (Mica2 and Mica2dot) and autonomous robot (Pioneer3)
    * Detect anomalous event in unknown environments using WSNs and a mobile robot
    * Video demonstration: sensor network detects abnormal situation with mobile robot responding to location of anomaly (2007)
2. Indoor wireless localization for mobile robots
    * Designed and implemented wireless indoor positioning system to locate mobile robots using triangulation and fingerprinting.

## Publications
* [Y. Li, and L. E. Parker, "Detecting and monitoring time-related abnormal events using a wireless sensor network and mobile robot", IEEE/RSJ International Conference on Intelligent Robots and Systems, IROS 2008, , Pages 3292-3298, Nice, France, 2008.](https://pdfs.semanticscholar.org/2522/3a2daf6cdd619dbd813cbafa611abf71b5d8.pdf)
**Abstract:**
In this paper, we present an anomaly detection system that is able to detect time-related anomalies by using a wireless sensor network and a mobile robot. The sensor network uses an unsupervised fuzzy Adaptive Resonance Theory (ART) neural  network  to  learn  and  detect  intruders  in  a  previously unknown environment. Upon the detection of an intruder, a mobile robot travels to the position where the intruder is detected to investigate by using its camera. The wireless sensor network uses  a hierarchical  communication/learning  structure,  where the  mobile  robot  is  the  root  node  of  the  tree.  Our  fuzzy  ART network is based on Kulakov and Davcev’s implementation [8]. However,  we  enhance  their  work  by  extending  the  fuzzy  ART neural  network  with  a  Markov  model  to  learn  a  time  series and  detect  time-related  anomalies.  Finally,  a  mobile  robot  is employed to verify whether the detected anomalies were caused by  intruders.  The  proposed  architecture  is  tested  on  physical hardware. Our results show that our enhanced detection system with mobile robot verification has a higher accuracy and lower false alarm  rate  than  the original  fuzzy  ART system.

* [Y. Li, and L. E. Parker, "Nearest neighbor imputation using spatial–temporal correlations in wireless sensor networks", IEEE/RSJ International Conference on Intelligent Robots and Systems, IROS 2008, , Pages 64-79, Nice, France, 2008.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5396980/)
**Abstract:**
Missing data is common in Wireless Sensor Networks (WSNs), especially with multi-hop communications. There are many reasons for this phenomenon, such as unstable wireless communications, synchronization issues, and unreliable sensors. Unfortunately, missing data creates a number of problems for WSNs. First, since most sensor nodes in the network are battery-powered, it is too expensive to have the nodes retransmit missing data across the network. Data re-transmission may also cause time delays when detecting abnormal changes in an environment. Furthermore, localized reasoning techniques on sensor nodes (such as machine learning algorithms to classify states of the environment) are generally not robust enough to handle missing data. Since sensor data collected by a WSN is generally correlated in time and space, we illustrate how replacing missing sensor values with spatially and temporally correlated sensor values can significantly improve the network’s performance. However, our studies show that it is important to determine which nodes are spatially and temporally correlated with each other. Simple techniques based on Euclidean distance are not sufficient for complex environmental deployments. Thus, we have developed a novel Nearest Neighbor (NN) imputation method that estimates missing data in WSNs by learning spatial and temporal correlations between sensor nodes. To improve the search time, we utilize a kd-tree data structure, which is a non-parametric, data-driven binary search tree. Instead of using traditional mean and variance of each dimension for kd-tree construction, and Euclidean distance for kd-tree search, we use weighted variances and weighted Euclidean distances based on measured percentages of missing data. We have evaluated this approach through experiments on sensor data from a volcano dataset collected by a network of Crossbow motes, as well as experiments using sensor data from a highway traffic monitoring application. Our experimental results show that our proposed 𝒦-NN imputation method has a competitive accuracy with state-of-the-art Expectation–Maximization (EM) techniques, while using much simpler computational techniques, thus making it suitable for use in resource-constrained WSNs.

* [Y. Li, and L. E. Parker, "Intruder detection using a wireless sensor network with an intelligent mobile robot response", IEEE Southeastcon, Pages 37-42, 2008.](https://ieeexplore.ieee.org/abstract/document/4494250/)
**Abstract:**
In this paper, we present an intruder detection system that uses a wireless sensor network and mobile robots. The sensor network uses an unsupervised fuzzy Adaptive Resonance Theory (ART) neural network to learn and detect intruders in a previously unknown environment. Upon the detection of an intruder, a mobile robot travels to the position where the intruder is detected to investigate. The wireless sensor network uses a hierarchical communication/learning structure, where the mobile robot is the root node of the tree. Our fuzzy ART network is based on Kulakov and Davcev’s implementation [6]. We enhanced the fuzzy ART neural network to learn a time-series and detect time-related changes using a Markov model. The proposed architecture is tested on physical hardware. Our results show that our enhanced detection system has a higher accuracy than the basic, original, fuzzy ART system.

* [Y. Li, and L. E. Parker, "Classification with missing data in a wireless sensor network", IEEE Southeastcon, Pages 533-538, 2008.](https://ieeexplore.ieee.org/abstract/document/4494352/)
**Abstract:**
We have developed a novel method to estimate missing observations in wireless sensor networks. We use a hierarchical unsupervised fuzzy ART neural network to represent the data cluster prototypes and describe missing input patterns based on the network. We then estimate missing inputs by a spatial-temporal imputation technique. Our experimental results show that our proposed approach performs better than nine other missing data imputation techniques including moving average and Expectation-Maximization (EM) imputation.


## Presentations

[presentation](../README.html)


