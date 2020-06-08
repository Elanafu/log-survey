# log-survey
Log survey paper list



# Log Mining

## Log Anomaly Detection

## Problems

### Root cause identification

1. [**COMPSAC19**] [Learning-based Anomaly Cause Tracing with Synthetic Analysis of Logs from Multiple Cloud Service Components](https://ieeecompsac.computer.org/2019/seta/)

## Methodology

### Supervised Approaches

#### Neural network-based

* ***LSTM model to predict the upcoming log events (workflow mining)***
  1. [**CCS17**] [DeepLog: Anomaly Detection and Diagnosis from System Logs through Deep Learning](https://www.cs.utah.edu/~lifeifei/papers/deeplog.pdf)
  1. [**IJCAI19**] [LogAnomaly: Unsupervised Detection of Sequential and Quantitative Anomalies in Unstructured Logs](https://www.ijcai.org/Proceedings/2019/0658.pdf)
1. [**MLCS18**] [Recurrent Neural Network Attention Mechanisms for Interpretable System Log Anomaly Detection](https://dl.acm.org/doi/pdf/10.1145/3217871.3217872)
  
* ***LSTM classification model to classify anomalies***
  1. [**FSE19**] [Robust Log-Based Anomaly Detection on Unstable Log Data](https://dl.acm.org/doi/pdf/10.1145/3338906.3338931)
  
  #### Graph Mining from Execution Logs
  
  1. [**KDD16**] [Anomaly Detection Using Program Control Flow Graph Mining from Execution Logs](https://www.kdd.org/kdd2016/papers/files/adf1233-nandiA.pdf)
#### Traditional machine learning-based

  * ***Clustering***
    1. [**IEEE/IFIP11**] [Mining Unstructured Log Files for Recurrent Fault Diagnosis](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5990536)
  * ***Decision Tree***
    1. [**ICAC04**] [Failure Diagnosis Using Decision Trees](https://people.eecs.berkeley.edu/~brewer/papers/icac2004_chen_diagnosis.pdf)
  2. [**JSS18**] [Execution anomaly detection in large-scale systems through console log analysis](https://freepaper.me/downloads/abstract/10.1016/j.jss.2018.05.016)
  * ***SVM***
    1. [**ICDM07**] [Failure prediction in ibm bluegene/l event logs](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4470294)
  * ***Logistic Regression***
    1. [**EuroSys10**] [Fingerprinting the datacenter: automated classification of performance crises](https://people.orie.cornell.edu/woodard/eurosys2010-paper97.pdf)

### Semi-supervised Approaches

- **PU Learning**
  1. [**IWQOS18**] [Device-Agnostic Log Anomaly Classification with Partial Labels](https://ieeexplore.ieee.org/abstract/document/8624141)

### Unsupervised Approaches

  * ***Clustering***
    1. [**ICSE16**] [Log Clustering based Problem Identification for Online Service Systems](https://dl.acm.org/doi/pdf/10.1145/2889160.2889232)
    1. [**FSE18**] [Identifying Impactful Service System Problems via Log Analysis](https://shilinhe.github.io/media/papers/fse18.pdf)
    1. [**SAC12**] [Spatio-temporal decomposition, clustering and identification for alert detection in system logs](https://dl.acm.org/doi/pdf/10.1145/2245276.2245395)
  * ***Statistics-based Detection***
    1. [**ICDM09**] [Execution Anomaly Detection in Distributed Systems through Unstructured Log Analysis](https://netman.aiops.org/~peidan/ANM2018Fall/6.LogAnomalyDetection/ReadingList/Execution%20anomaly%20detection%20in%20distributed%20systems%20through%20unstructured%20log%20analysis.pdf)
    1. [**KDD05**] [Dynamic Syslog Mining for Network Failure Monitoring](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.96.8083&rep=rep1&type=pdf)
    1. [**ICDM08**] [Alert Detection in System Logs](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4781208)
* **Autoencoder**
  1. [**DM19**] [Anomaly Detection From Log Files Using Unsupervised Deep Learning](https://homes.di.unimi.it/cuculo/papers/bursic2019anomaly.pdf)
   * ***PCA***
   1. [ICML10] [Detecting Large-Scale System Problems by Mining Console Logs](https://people.eecs.berkeley.edu/~jordan/papers/xu-etal-icml10.pdf)
