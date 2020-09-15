<p align="center"> <a href="https://github.com/logpai"> <img src="https://github.com/logpai/logpai.github.io/blob/master/img/logpai_logo.jpg" width="425"></a></p>

# Awesome Log Analysis Research
A curated list of awesome publications on log analysis.


Table of Contents

- [Awesome Log Analysis Research](#awesome-log-analysis-research)
  - [Conferences and Journals](#conferences-and-journals)
  - [Competitions](#competitions)
  - [Datasets](#datasets)
  - [Research Groups](#research-groups)
  - [Logging](#logging)
    - [By static analysis](#by-static-analysis)
    - [By statistical methods](#by-statistical-methods)
    - [Empirical Study](#empirical-study)
    - [Pending Classification](#pending-classification)
  - [Log Compression](#log-compression)
    - [Bucket](#bucket)
    - [Dictionary](#dictionary)
    - [Statistics](#statistics)
    - [Others](#others)
  - [Log Parsing](#log-parsing)
    - [Offline](#offline)
    - [Online](#online)
  - [Log Mining](#log-mining)
    - [*Pending*](#pending)
    - [Anomaly Detection](#anomaly-detection)
      - [Supervised Approaches](#supervised-approaches)
      - [Semi-supervised Approaches](#semi-supervised-approaches)
      - [Unsupervised Approaches](#unsupervised-approaches)
    - [Failure Prediction](#failure-prediction)
    - [Failure Diagnosis](#failure-diagnosis)
    - [Others](#others-1)
  - [Credits](#credits)
  - [Contributions](#contributions)
  - [License](#license)

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


## Logging

### By static analysis

- [MSR 2019] [Tracing Back Log Data to its Log Statement: From Research to Practice](https://pure.tudelft.nl/portal/files/52060635/paper.pdf)
- [ICSE 2019] [DLFinder: Characterizing and Detecting Duplicate Logging Code Smells](https://users.encs.concordia.ca/~shang/pubs/icse2019_zhenhao.pdf)
- [SOSP 2017] [Log20: Fully Automated Optimal Placement of Log Printing Statements under Specified Overhead Threshold](http://log20.dsrg.utoronto.ca/log20_sosp17_paper.pdf)
- [ICSE 2017] [Characterizing and Detecting Anti-patterns in the Logging Code](https://dl.acm.org/doi/pdf/10.1109/ICSE.2017.15)
- [OSDI 2012] [Be Conservative: Enhancing Failure Diagnosis with Proactive Logging](https://www.eecg.utoronto.ca/~yuan/papers/osdi12-errlog.pdf)
- [ICSE 2012] [Characterizing logging practices in open-source software](http://petertsehsun.github.io/soen691/current/papers/log_icse12.pdf)
- [ASPLOS 2011] [Improving Software Diagnosability via Log Enhancement](http://opera.ucsd.edu/paper/asplos11-logenhancer.pdf)

### By statistical methods

- [TSE19liu] [Which Variables Should I Log?](https://xin-xia.github.io/publication/tse197.pdf)
- [ASE18He] [Characterizing the Natural Language Descriptions in Software Logging Statements](https://pinjiahe.github.io/papers/ASE18.pdf)
- [ATC15Ding] [Log2 : A Cost-Aware Logging Mechanism for Performance Diagnosis](https://www.usenix.org/system/files/conference/atc15/atc15-paper-ding.pdf)

### Empirical Study

- [ICSE15Pecchia] [Industry practices and event logging: assessment of a critical software development process](https://dl.acm.org/doi/10.5555/2819009.2819035)
- [ICSE12Shang] [Bridging the Divide between Software Developers and Operators using Logs](https://users.encs.concordia.ca/~shang/pubs/icse2012_Shang.pdf)

### Pending Classification

- [OSDI18Lockerman] [The FuzzyLog: A Partially Ordered Shared Log](https://www.usenix.org/conference/osdi18/presentation/lockerman)
- [ICSME19Zhi] [An Exploratory Study of Logging Configuration Practice in Java](http://taoxie.cs.illinois.edu/publications/icsme19-log.pdf)
- [SOSP13] [Tango: distributed data structures over a shared log](https://dl.acm.org/doi/10.1145/2517349.2522732)
- [ICSDCS18] [SLoG: Large-Scale Logging Middleware for HPC and Big Data Convergence](https://ieeexplore.ieee.org/document/8416419)
- [ICDCS10] [Visual, Log-Based Causal Tracing for Performance Debugging of MapReduce Systems](https://ieeexplore.ieee.org/document/5541622)
- [ICSE20] [Studying the Use of Java Logging Utilities in the Wild](https://www.eecs.yorku.ca/~chenfsd/resources/icse2020_chen.pdf)

## Log Compression

### Bucket
- [IPDPS 2006] [Lossless compression for large scale cluster logs](https://ieeexplore.ieee.org/document/1639692)
- [ADBIS 2007] [Fast and efficient log file compression](http://www.adbis.org/docs/lp/6.pdf)
- [ICSE 2008] [An Industrial Case Study of Customizing Operational Profiles Using Log Compression](https://dl.acm.org/doi/abs/10.1145/1368088.1379445)
- [SIGMOD 2013] [Adaptive log compression for massive log data](https://dl.acm.org/doi/10.1145/2463676.2465341)
- [IEEE Trustcom/BigDataSE/ISPA 2016] [MLC: An Efficient Multi-level Log Compression Method for Cloud Backup Systems](https://ieeexplore.ieee.org/document/7847098/)
  
### Dictionary
- [TCSET 2008] [Sub-atomic field processing for improved web log compression](https://ieeexplore.ieee.org/document/5423436)
- [CCGRID 2015] [Cowic: A column-wise independent compression for log stream analysis](https://ieeexplore.ieee.org/document/7152468)
- [IMCC 2014] [Lightweight Packing of Log Files for Improved Compression in Mobile Tactical Networks](https://ieeexplore.ieee.org/document/6956758)
- [DCC 2004] [High density compression of log files](https://ieeexplore.ieee.org/document/1281533)

### Statistics
- [DaWaK 2003] [Comprehensive Log Compression with Frequent Patterns](https://link.springer.com/chapter/10.1007/978-3-540-45228-7_36)
- [ICEIS 2019] [Rough Logs: A Data Reduction Approach for Log Files](https://www.scitepress.org/Papers/2019/77351/pdf/index.html)
- [ASE 2019] [Logzip: extracting hidden structures via iterative clustering for log compression](https://arxiv.org/abs/1910.00409)

### Others
- [EMSE 2019] [A Study of the Performance of General Compressors on Log Files](https://users.encs.concordia.ca/~shang/pubs/Kundi_EMSE2020.pdf)
- [Ph.D. Dissertation 2008] [Using semantic knowledge to improve compression on log files](https://homes.cs.ru.ac.za/B.Irwin/theses/Otten%202008%20%20Msc%20Using%20semantic%20knowledge%20to%20improve%20compression%20on%20log%20files.pdf)


## Log Parsing

### Offline
- [IPOM'03] [A Data Clustering Algorithm for Mining Patterns from Event Logs](http://www.quretec.com/u/vilo/edu/2003-04/DM_seminar_2003_II/ver1/P12/slct-ipom03-web.pdf)
- [QSIC'08] [Abstracting Execution Logs to Execution Events for Enterprise Applications](https://www.researchgate.net/publication/4366728_Abstracting_Execution_Logs_to_Execution_Events_for_Enterprise_Applications_Short_Paper)
- [ICDM'09] [Execution Anomaly Detection in Distributed Systems through Unstructured Log Analysis](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/DM790-CR.pdf)
- [MSR'10] [Abstracting Log Lines to Log Event Types for Mining Software System Logs](http://www.se.rit.edu/~mei/publications/pdfs/Abstracting-Log-Lines-to-Log-Event-Types-for-Mining-Software-System-Logs.pdf)
- [CIKM'11] [LogSig: Generating System Events from Raw Textual Logs](https://users.cs.fiu.edu/~taoli/pub/liang-cikm2011.pdf) 
- [KDD'09] [Clustering Event Logs Using Iterative Partitioning](https://web.cs.dal.ca/~makanju/publications/paper/kdd09.pdf)
- [CNSM'15] [LogCluster - A Data Clustering and Pattern Mining Algorithm for Event Logs](http://dl.ifip.org/db/conf/cnsm/cnsm2015/1570161213.pdf)
- [CIKM'16] [LogMine: Fast Pattern Recognition for Log Analytics](http://www.cs.unm.edu/~mueen/Papers/LogMine.pdf)
- [TDSC'18] [Towards Automated Log Parsing for Large-Scale Log Data Analysis](https://pinjiahe.github.io/papers/TDSC17.pdf)
- [ICPC'18] [A Search-based Approach for Accurate Identification of Log Message Formats](http://publications.uni.lu/bitstream/10993/35286/1/ICPC-2018.pdf)

### Online
- [SCC'13] [Incremental Mining of System Log Format](http://ieeexplore.ieee.org/document/6649746/)
- [CNSM'15] [Length Matters: Clustering System Log Messages using Length of Words](https://arxiv.org/pdf/1611.03213.pdf)
- [ICDM'16] [Spell: Streaming Parsing of System Event Logs](https://www.cs.utah.edu/~lifeifei/papers/spell.pdf)
- [ICWS'17] [Drain: An Online Log Parsing Approach with Fixed Depth Tree](https://jiemingzhu.github.io/pub/pjhe_icws2017.pdf)
- [arXiv'18] [A Directed Acyclic Graph Approach to Online Log Parsing](https://arxiv.org/abs/1806.04356)
- [TSE'20] [Logram: Efficient Log Parsing Using n-Gram Dictionaries](https://arxiv.org/abs/2001.03038)


## Log Mining

### *Pending*

- [SOSP09Xu] [Detecting large-scale system problems by mining console logs](https://dl.acm.org/doi/10.1145/1629575.1629587)
- [ATC11] [In-situ MapReduce for Log Processing](https://www.usenix.org/conference/usenixatc11/situ-mapreduce-log-processing)
- [ATC10] [Mining Invariants from Console Logs for System Problem Detection](https://www.usenix.org/conference/usenix-atc-10/mining-invariants-console-logs-system-problem-detection)
- [ICDCS18] [LogLens: A Real-Time Log Analysis System](https://ieeexplore.ieee.org/document/8416368)
- 

### Anomaly Detection

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


### Failure Prediction

### Failure Diagnosis
- XX 
  - [COMPSAC19] [Learning-based Anomaly Cause Tracing with Synthetic Analysis of Logs from Multiple Cloud Service Components](https://ieeecompsac.computer.org/2019/seta/)

### Others




## Credits
- Inspired by [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning).


## Contributions
how to contribute to this repo

## License
the repo will be under the MIT license.
