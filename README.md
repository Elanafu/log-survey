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
    - [Delta encoding](#delta-encoding)
    - [Bucketing](#bucketing)
    - [Text replacement](#text-replacement)
    - [Log transposition](#log-transposition)
    - [Others](#others)
  - [Log Parsing](#log-parsing)
    - [Offline](#offline)
    - [Online](#online)
    - [Benchmark and Tools](#benchmark-and-tools)
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

### Where to log

- [OSDI 2012] [Be Conservative: Enhancing Failure Diagnosis with Proactive Logging](https://www.eecg.utoronto.ca/~yuan/papers/osdi12-errlog.pdf)
- [TSE 2013] [Event Logs for the Analysis of Software Failures: A Rule-Based Approach](http://ieeexplore.ieee.org/document/6320555/)
- [ICSE 2015] [Learning to Log: Helping Developers Make Informed Logging Decisions](http://ieeexplore.ieee.org/document/7194593/)
- [ICSE 2015] [Where do developers log? an empirical study on logging practices in industry]http://dl.acm.org/citation.cfm?doid=2591062.2591175()
- [ATC 2015] [Log2 : A Cost-Aware Logging Mechanism for Performance Diagnosis](https://www.usenix.org/system/files/conference/atc15/atc15-paper-ding.pdf)
- [SOSP 2017] [Log20: Fully Automated Optimal Placement of Log Printing Statements under Specified Overhead Threshold](http://log20.dsrg.utoronto.ca/log20_sosp17_paper.pdf)
- [HotOS 2017] [The Game of Twenty Questions: Do You Know Where to Log?](https://dl.acm.org/doi/10.1145/3102980.3103001)
- [ASE 2020] [Where Shall We Log? Studying and Suggesting Logging Locations in Code Blocks](https://users.encs.concordia.ca/~shang/pubs/Zhenhao_ASE20.pdf)

### What to log

- [ASPLOS 2011] [Improving Software Diagnosability via Log Enhancement](http://opera.ucsd.edu/paper/asplos11-logenhancer.pdf)
- [ASE 2018] [Characterizing the Natural Language Descriptions in Software Logging Statements](https://pinjiahe.github.io/papers/ASE18.pdf)
- [TSE 2019] [Which Variables Should I Log?](https://xin-xia.github.io/publication/tse197.pdf)
- [ICPC 2019] [PADLA: a dynamic log level adapter using online phase detection](https://sel.ist.osaka-u.ac.jp/lab-db/betuzuri/archive/1157/1157.pdf)

### How to log

- [ECOOP 1997] [Aspect-oriented programming](https://www.cs.ubc.ca/~gregor/papers/kiczales-ECOOP1997-AOP.pdf)
- [DSN 2010] [Assessing and improving the effectiveness of logs for the analysis of software faults](http://ieeexplore.ieee.org/document/5544279/)
- [ICSE 2012] [Characterizing logging practices in open-source software](http://petertsehsun.github.io/soen691/current/papers/log_icse12.pdf)
- [ICSME 2014] [Understanding Log Lines Using Development Knowledge](http://ieeexplore.ieee.org/document/6976068/)
- [ICSE 2015] [Industry practices and event logging: assessment of a critical software development process](https://dl.acm.org/doi/10.5555/2819009.2819035)
- [ESE 2015] [Studying the relationship between logging characteristics and the code quality of platform software](http://link.springer.com/10.1007/s10664-013-9274-8)
- [ICSE 2017] [Characterizing and Detecting Anti-patterns in the Logging Code](https://dl.acm.org/doi/pdf/10.1109/ICSE.2017.15)
- [OSDI 2018] [The FuzzyLog: A Partially Ordered Shared Log](https://www.usenix.org/conference/osdi18/presentation/lockerman)
- [ATC 2018] [Troubleshooting Transiently-Recurring Errors in Production Systems with Blame-Proportional Logging](https://www.usenix.org/system/files/conference/atc18/atc18-luo.pdf)
- [ATC 2018] [NanoLog: A Nanosecond Scale Logging System](https://www.usenix.org/system/files/conference/atc18/atc18-yang.pdf)
- [NSDI 2018] [Carousel: Scalable Logging for Intrusion Prevention Systems](https://www.usenix.org/conference/nsdi10-0/carousel-scalable-logging-intrusion-prevention-systems)
- [ICSE 2019] [DLFinder: Characterizing and Detecting Duplicate Logging Code Smells](https://users.encs.concordia.ca/~shang/pubs/icse2019_zhenhao.pdf)
- [ICSE 2016] [The bones of the system: a case study of logging and telemetry at Microsoft](http://dl.acm.org/citation.cfm?doid=2889160.2889231)
- [MSR 2016] [Logging library migrations: a case study for the apache software foundation projects](http://dl.acm.org/citation.cfm?doid=2901739.2901769)
- [ESE 2017] [Characterizing logging practices in Java-based open source software projects - a replication study in Apache Software Foundation](http://link.springer.com/10.1007/s10664-016-9429-5)
- [ESE 2018] [Studying and detecting log-related issues](http://link.springer.com/10.1007/s10664-018-9603-z)
- [ESE 2018] [Examining the stability of logging statements](http://link.springer.com/10.1007/s10664-017-9518-0)
- [ESE 2018] [An exploratory study on assessing the energy impact of logging on Android applications](https://www.eecs.yorku.ca/~zmjiang/publications/emse2017_chowdhury.pdf)
- [ESE 2019] [Studying the characteristics of logging practices in mobile apps: a case study on F-Droid](http://link.springer.com/10.1007/s10664-019-09687-9)
- [ICSE 2020] [Studying the Use of Java Logging Utilities in the Wild](http://www.cse.yorku.ca/~zmjiang/publications/icse2020_chen.pdf)


## Log Compression

### Delta encoding
- Lossless compression for large scale cluster logs
- MLC: An Efficient Multi-level Log Compression Method for Cloud Backup Systems
- Fast and efficient log file compression
- Felfcnca: Fast & efficient log file com- pression using non linear cellular automata classifier.

### Bucketing
- Adaptive log compression for massive log data
- Mlc: An efficient multi-level log compression method for cloud backup systems.
  
### Text replacement
- Evaluating text preprocessing to im- prove compression on maillogs.
- Using semantic knowledge to improve compression on log files. [Thesis]
- An Industrial Case Study of Customizing Operational Profiles Using Log Compression
- Rough Logs: A Data Reduction Approach for Log Files
  
### Log transposition
- Sub-atomic field processing for improved web log compression
- Cowic: A column-wise independent compression for log stream analysis
logzip
- Lightweight Packing of Log Files for Improved Compression in Mobile Tactical Networks
- An Industrial Case Study of Customizing Operational Profiles Using Log Compression
- Comprehensive Log Compression with Frequent Patterns

### Others
- A Study of the Performance of General Compressors on Log Files
- Immutable Log Storage as a Service [with blockchain]
- Anonymization of System Logs for Privacy and Storage Benefits

## Log Parsing

### Offline
- [IPOM'03] [A Data Clustering Algorithm for Mining Patterns from Event Logs](http://www.quretec.com/u/vilo/edu/2003-04/DM_seminar_2003_II/ver1/P12/slct-ipom03-web.pdf)
- [QSIC'08] [Abstracting Execution Logs to Execution Events for Enterprise Applications](https://www.researchgate.net/publication/4366728_Abstracting_Execution_Logs_to_Execution_Events_for_Enterprise_Applications_Short_Paper)
- [ICDM'09] [Execution Anomaly Detection in Distributed Systems through Unstructured Log Analysis](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/DM790-CR.pdf)
- [MSR'10] [Abstracting Log Lines to Log Event Types for Mining Software System Logs](http://www.se.rit.edu/~mei/publications/pdfs/Abstracting-Log-Lines-to-Log-Event-Types-for-Mining-Software-System-Logs.pdf)
- [CIKM'11] [LogSig: Generating System Events from Raw Textual Logs](https://users.cs.fiu.edu/~taoli/pub/liang-cikm2011.pdf) 
- [KDD'09] [Clustering Event Logs Using Iterative Partitioning](https://web.cs.dal.ca/~makanju/publications/paper/kdd09.pdf)
- [TKDE'12] [A Lightweight Algorithm for Message Type Extraction in System Application Logs](https://ieeexplore.ieee.org/document/5936060)
- [CNSM'15] [LogCluster - A Data Clustering and Pattern Mining Algorithm for Event Logs](http://dl.ifip.org/db/conf/cnsm/cnsm2015/1570161213.pdf)
- [CIKM'16] [LogMine: Fast Pattern Recognition for Log Analytics](http://www.cs.unm.edu/~mueen/Papers/LogMine.pdf)
- [TDSC'18] [Towards Automated Log Parsing for Large-Scale Log Data Analysis](https://pinjiahe.github.io/papers/TDSC17.pdf)
- [ICPC'18] [A Search-based Approach for Accurate Identification of Log Message Formats](http://publications.uni.lu/bitstream/10993/35286/1/ICPC-2018.pdf)

### Online
- [SCC'13] [Incremental Mining of System Log Format](http://ieeexplore.ieee.org/document/6649746/)
- [arXiv'15] [Length Matters: Clustering System Log Messages using Length of Words](https://arxiv.org/pdf/1611.03213.pdf)
- [TKDE'19] [Spell: Online Streaming Parsing of Large Unstructured System Logs](https://ieeexplore.ieee.org/document/8489912)
- [ICWS'17] [Drain: An Online Log Parsing Approach with Fixed Depth Tree](https://jiemingzhu.github.io/pub/pjhe_icws2017.pdf)
- [arXiv'18] [A Directed Acyclic Graph Approach to Online Log Parsing](https://arxiv.org/abs/1806.04356)
- [TSE'20] [Logram: Efficient Log Parsing Using n-Gram Dictionaries](https://arxiv.org/abs/2001.03038)

### Benchmark and Tools
- [ICSE-SEIP'19] [Tools and benchmarks for automated log parsing](https://arxiv.org/abs/1811.03509)



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

- [MACS18] [PreFix: Switch failure prediction in datacenter networks](https://doi.org/10.1145/3179405)
- [HPDC18] [Desh: deep learning for system health prediction of lead times to failure in HPC](https://doi.org/10.1145/3208040.3208051)
- [KDD03] [Critical event prediction for proactive management in large-scale computer clusters](https://doi.org/10.1145/956750.956799)
- [IPDPS20] [Aarohi: Making real-time node failure prediction feasible](https://doi.org/10.1109/IPDPS47924.2020.00115)
- [CLUSTER17] [Data Mining-Based Analysis of HPC Center Operations](https://doi.org/10.1109/CLUSTER.2017.23)
- [CLUSTER14] [Exploring void search for fault detection on extreme scale systems](https://doi.org/10.1109/CLUSTER.2014.6968757)
- [WWW19] [Outage Prediction and Diagnosis for Cloud Service Systems](http://dl.acm.org/citation.cfm?doid=3308558.3313501)
- [FSE18] [Predicting Node failure in cloud service systems](http://dl.acm.org/citation.cfm?doid=3236024.3236060)
- [FSE19] [Latent error prediction and fault localization for microservice applications by learning from system trace logs](http://dl.acm.org/citation.cfm?doid=3338906.3338961)

### Failure Diagnosis
- XX 
  - [COMPSAC19] [Learning-based Anomaly Cause Tracing with Synthetic Analysis of Logs from Multiple Cloud Service Components](https://ieeecompsac.computer.org/2019/seta/)

### Others

- [DSN14] [Mining Historical Issue Repositories to Heal Large-Scale Online Service Systems](https://doi.org/10.1109/DSN.2014.39)
- [ASE98] [Testing using log file analysis: Tools, methods, and issues](https://doi.org/10.1109/ASE.1998.732614)
- [ASE18] [An automated approach to estimating code coverage measures via execution logs](https://doi.org/10.1145/3238147.3238214)
- [ASE19] [An experience report of generating load tests using log-recovered workloads at varying granularities of user behaviour](https://doi.org/10.1109/ASE.2019.00068)
- [ASE15] [Have we seen enough traces? (T)](https://doi.org/10.1109/ASE.2015.62)
- [ICSE08] [An approach to detecting duplicate bug reports using natural language and execution information](https://doi.org/10.1145/1368088.1368151)


## Credits
- Inspired by [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning).


## Contributions
how to contribute to this repo

## License
the repo will be under the MIT license.
