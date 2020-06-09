# log-survey
Log survey paper list



## Contents
  - [Conferences and Journals](#conferences-and-journals)
  - [Competitions](#competitions)
  - [Datasets](#datasets)
  - [Research Groups](#research-groups)
  - [Logging Statements & Logging Practices](#logging-statements--logging-practices)
    - [Category 1](#category-1)
    - [Category 2](#category-2)
  - [Log Parsing](#log-parsing)
    - [Category 1](#category-1-1)
    - [Category 2](#category-2-1)
  - [Log Mining](#log-mining)
    - [Log Anomaly Detection](#log-anomaly-detection)
      - [Supervised Approaches](#supervised-approaches)
      - [Semi-supervised Approaches](#semi-supervised-approaches)
      - [Unsupervised Approaches](#unsupervised-approaches)
    - [Problems Identification](#problems-identification)
    - [Root cause identification](#root-cause-identification)
  - [Debugging and Diagnosis](#debugging-and-diagnosis)
  - [Log File Storage](#log-file-storage)

## Conferences and Journals
Logs are a type of valuable data generated from many sources such as software, systems, networks, devices, etc. They have also been used for a number of tasks related to reliability, security, performance, and energy. Therefore, the research of log analysis has attracted interests from different research areas.

+ **System area**
    + Conferences: [OSDI](https://dblp.uni-trier.de/db/conf/osdi/index) | [SOSP](https://dblp.uni-trier.de/db/conf/sosp/index) | [ATC](https://dblp.uni-trier.de/db/conf/usenix/index) | [ICDCS](https://dblp.uni-trier.de/db/conf/icdcs/index)
    + Journals: [TC](https://dblp.uni-trier.de/db/journals/tc/index.html) | [TOCS](https://dblp.uni-trier.de/db/journals/tocs/index) | [TPDS](https://dblp.uni-trier.de/db/journals/tpds/index.html)
+ **Cloud computing area**
    + Conferences: [SoCC](https://dblp.uni-trier.de/db/conf/cloud/index.html) | [CLOUD](https://dblp.uni-trier.de/db/conf/IEEEcloud/index)
    + Journals: [TCC](https://dblp.uni-trier.de/db/journals/tcc/index.html)
+ **Networking area**
    + Conferences: [NSDI](https://dblp.uni-trier.de/db/conf/nsdi/index) | [INFOCOMM](https://dblp.uni-trier.de/db/conf/infocom/index)
    + Journals: [TON](https://dblp.uni-trier.de/db/journals/ton/index.html)
+ **Software engineering area**
    + Conferences: [ICSE](https://dblp.uni-trier.de/db/conf/icse/index) | [FSE](https://dblp.uni-trier.de/db/conf/sigsoft/index) | [ASE](https://dblp.org/db/conf/kbse/index.html)
    + Journals: [TSE](https://dblp.org/db/journals/tse/index) | [TOSEM](https://dblp.uni-trier.de/db/journals/tosem/index)
+ **Reliability area**
    + Conferences: [DSN](https://dblp.uni-trier.de/db/conf/dsn/index) | [ISSRE](https://dblp.uni-trier.de/db/conf/issre/index.html) | [SRDS](https://dblp.uni-trier.de/db/conf/srds/index)
    + Journals: [TDSC](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8858) | [TR](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=24)
+ **Security area**
    + Conferences: [CCS](http://www.wikicfp.com/cfp/servlet/event.showcfp?eventid=83847) | [DSN](http://www.dsn.org/)
    + Journals: [TDSC](https://dblp.uni-trier.de/db/journals/tdsc/index.html)
+ **AI and Bigdata area**
    + Conferences: [KDD](https://dblp.uni-trier.de/db/conf/kdd/index) | [CIKM](https://dblp.uni-trier.de/db/conf/cikm/index) | [ICDM](https://dblp.uni-trier.de/db/conf/icdm/index) | [BigData](https://dblp.org/db/conf/bigdataconf/index)
    + Journals: [TKDE](https://dblp.uni-trier.de/db/journals/tkde/index) | [TBD](https://dblp.uni-trier.de/db/journals/tbd/index.html)
+ **Industrial conferences**
    + [SREcon](https://www.usenix.org/conferences/byname/925) | [GOPS](https://www.bagevent.com/event/GOPS2019-shenzhen?bag_track=bagevent)
  
## Competitions

XXXX 

## Datasets

Loghub

## Research Groups
| China (& HK) | ||||
| :---------| :------ | :------ | :------ | :------ |
| [Michael R. Lyu](http://www.cse.cuhk.edu.hk/lyu/), CUHK | [Dongmei Zhang](https://www.microsoft.com/en-us/research/people/dongmeiz/), Microsoft | [Pengfei Chen](http://sdcs.sysu.edu.cn/content/3747), SYSU | [Dan Pei](https://netman.aiops.org/~peidan/), Tsinghua | |
| **USA** |||||
| [Yuanyuan Zhou](https://cseweb.ucsd.edu/~yyzhou/), UCSD | [Tao Xie](http://taoxie.cs.illinois.edu/), UIUC | [Dawson Engler](http://web.stanford.edu/~engler/), Stanford | [Ben Liblit](http://pages.cs.wisc.edu/~liblit/#bug-isolation), Wisconsin–Madison ||
| **Canada** |||||
| [Ding Yuan](http://www.eecg.toronto.edu/~yuan/Home.html), Toronto University | [Ahmed E. Hassan](http://research.cs.queensu.ca/~ahmed/home/), Queen's University | [Weiyi Shang](https://users.encs.concordia.ca/~shang/), Concordia University |[Zhen Ming (Jack) Jiang](http://www.cse.yorku.ca/~zmjiang/), York University||
| **UK** |||||
|  |||||
| **Europe** |||||
| **Australia** |||||
| [Ingo Weber](https://people.csiro.au/W/I/Ingo-Weber), CSIRO |||||

## Papers

## Logging Statements & Logging Practices

### Log Compression

#### Delta encoding
- Lossless compression for large scale cluster logs
- MLC: An Efficient Multi-level Log Compression Method for Cloud Backup Systems
- Fast and efficient log file compression
- Felfcnca: Fast & efficient log file com- pression using non linear cellular automata classifier.
#### Bucketing
- Adaptive log compression for massive log data
- Mlc: An efficient multi-level log compression method for cloud backup systems.
  
#### Text replacement
- Evaluating text preprocessing to im- prove compression on maillogs.
- Using semantic knowledge to improve compression on log files. [Thesis]
- An Industrial Case Study of Customizing Operational Profiles Using Log Compression
- Rough Logs: A Data Reduction Approach for Log Files
  
#### Log transposition
- Sub-atomic field processing for improved web log compression
- Cowic: A column-wise independent compression for log stream analysis
logzip
- Lightweight Packing of Log Files for Improved Compression in Mobile Tactical Networks
- An Industrial Case Study of Customizing Operational Profiles Using Log Compression
- Comprehensive Log Compression with Frequent Patterns

#### Others
- A Study of the Performance of General Compressors on Log Files
- Immutable Log Storage as a Service [with bloch chain]
- Anonymization of System Logs for Privacy and Storage Benefits

## Log Parsing

### Category 1
### Category 2

## Log Mining

### Log Anomaly Detection

#### Supervised Approaches

* Neural network-based
  - [CCS17] [DeepLog: Anomaly Detection and Diagnosis from System Logs through Deep Learning](https://www.cs.utah.edu/~lifeifei/papers/deeplog.pdf)
  - [IJCAI19] [LogAnomaly: Unsupervised Detection of Sequential and Quantitative Anomalies in Unstructured Logs](https://www.ijcai.org/Proceedings/2019/0658.pdf)
  - [MLCS18] [Recurrent Neural Network Attention Mechanisms for Interpretable System Log Anomaly Detection](https://dl.acm.org/doi/pdf/10.1145/3217871.3217872)
  - [FSE19] [Robust Log-Based Anomaly Detection on Unstable Log Data](https://dl.acm.org/doi/pdf/10.1145/3338906.3338931)

- Graph Mining
  - [KDD16] [Anomaly Detection Using Program Control Flow Graph Mining from Execution Logs](https://www.kdd.org/kdd2016/papers/files/adf1233-nandiA.pdf)

- Traditional machine learning-based
  - [IEEE/IFIP11] [Mining Unstructured Log Files for Recurrent Fault Diagnosis](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=5990536)
  - [ICAC04] [Failure Diagnosis Using Decision Trees](https://people.eecs.berkeley.edu/~brewer/papers/icac2004_chen_diagnosis.pdf)
  - [JSS18] [Execution anomaly detection in large-scale systems through console log analysis](https://freepaper.me/downloads/abstract/10.1016/j.jss.2018.05.016)
  - [ICDM07] [Failure prediction in ibm bluegene/l event logs](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4470294)
  - [EuroSys10] [Fingerprinting the datacenter: automated classification of performance crises](https://people.orie.cornell.edu/woodard/eurosys2010-paper97.pdf)

#### Semi-supervised Approaches

- PU Learning

  - [IWQOS18] [Device-Agnostic Log Anomaly Classification with Partial Labels](https://ieeexplore.ieee.org/abstract/document/8624141)

#### Unsupervised Approaches
  - Clustering
    - [ICSE16] [Log Clustering based Problem Identification for Online Service Systems](https://dl.acm.org/doi/pdf/10.1145/2889160.2889232)
    - [FSE18] [Identifying Impactful Service System Problems via Log Analysis](https://shilinhe.github.io/media/papers/fse18.pdf)
    - [SAC12] [Spatio-temporal decomposition, clustering and identification for alert detection in system logs](https://dl.acm.org/doi/pdf/10.1145/2245276.2245395)
  - Statistics-based Detection
    - [ICDM09] [Execution Anomaly Detection in Distributed Systems through Unstructured Log Analysis](https://netman.aiops.org/~peidan/ANM2018Fall/6.LogAnomalyDetection/ReadingList/Execution%20anomaly%20detection%20in%20distributed%20systems%20through%20unstructured%20log%20analysis.pdf)
    - [KDD05] [Dynamic Syslog Mining for Network Failure Monitoring](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.96.8083&rep=rep1&type=pdf)
    - [ICDM08] [Alert Detection in System Logs](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4781208)

- Autoencoder
  - [DM19] [Anomaly Detection From Log Files Using Unsupervised Deep Learning](https://homes.di.unimi.it/cuculo/papers/bursic2019anomaly.pdf)
- PCA
  - [ICML10] [Detecting Large-Scale System Problems by Mining Console Logs](https://people.eecs.berkeley.edu/~jordan/papers/xu-etal-icml10.pdf)


### Problems Identification

### Root cause identification
- XX 
  - [COMPSAC19] [Learning-based Anomaly Cause Tracing with Synthetic Analysis of Logs from Multiple Cloud Service Components](https://ieeecompsac.computer.org/2019/seta/)



## Debugging and Diagnosis

### Empirical Study
Understanding Customer Problem Troubleshooting from Storage System Logs

[ICSE'19] An Empirical Study On Leveraging Logs For Debugging Production Failures

Insights into the Diagnosis of System Failures from Cluster Message Logs

## Log File Storage


## Credits
- Inspired by [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning).


## Contributions
how to contribute to this repo

## License
the repo will be under the MIT license.