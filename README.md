# Paper4OLTPandConcurrencyTesting

This repository lists papers with topics covering OLTP and error testing (especially concurrency-related testing).

New PR is welcome for any material that you think should be included in this collection.  .

If you want to add new paper, please follow link format: 

```markdown
paperName(with access link) [MeetingName(with open source code, if exists) Year]
```

- [Paper For OLTP and ConcurrencyTesting](#paper4oltpandconcurrencytesting)
  - [Survey](#survey)
  - [OLTP](#oltp)
    - [Implementation](#implementation)
    - [Concurrency Control](#concurrency-control)
    - [Transaction](#transaction)
    - [Anomaly Detection](#anomaly-detection)
    - [Benchmark](#benchmark)
  - [Testing](#testing)
    - [Concurrency Testing](#concurrency-testing)
    - [Fuzzing](#fuzzing)
    - [Root Cause Analyze](#root-cause-analyze)
    - [Fault Location](#fault-location)

## Survey

- [10 Years of research on debugging concurrent and multicore software: a systematic mapping study](http://link.springer.com/10.1007/s11219-015-9301-7) [Software Quality Journal 17]

## OLTP

### Implementation

- GeoGauss: Strongly Consistent Coordinator-Free OLTP for Geo-Replicated SQL Database  [SIGMOD 23]
- [P4DB - The Case for In-Network OLTP]( https://doi.org/10.1145/3514221.3517825 ) [SIGMOD 22]
- [GaccO - A GPU-accelerated OLTP DBMS ]( https://doi.org/10.1145/3514221.3517876 )[SIGMOD 22]
- [Proteus: Autonomous Adaptive Storage for Mixed Workloads]( https://doi.org/10.1145/3514221.3517834 ) [SIGMOD 22]

### Concurrency Control

-  Polaris: Enabling Transaction Priority in Optimistic Concurrency Control [SIGMOD 23]
- [Diva: Making MVCC Systems HTAP-Friendly]( https://doi.org/10.1145/3514221.3526135 ) [SIGMOD 22]
- [Plor: General Transactions with Predictable, Low Tail Latency]( https://doi.org/10.1145/3514221.3517879 ) [SIGMOD 22]

### Transaction

-  Transaction Scheduling: From Conflicts to Runtime Conflicts [SIGMOD 23]
-  [Towards a Practical Database Management System with Verifiable ACID Properties and Transaction Correctness]( https://doi.org/10.1145/3514221.3517851 ) [SIGMOD 22]
-  [Skeena: Efficient and Consistent Cross-Engine Transactions]( https://doi.org/10.1145/3514221.3526171 ) [SIGMOD 22]
-  [Natto: Providing Distributed Transaction Prioritization for High-Contention Workloads]( https://doi.org/10.1145/3514221.3526161 ) [SIGMOD 22]

### Anomaly Detection

-  [Robust and Transferable Log-based Anomaly Detection](http://arxiv.org/abs/2102.11570)   [SIGMOD 23] 
- [Detecting Isolation Bugs via Transaction Oracle Construction]( https://doi.org/10.5281/zenodo.7645649 ) [[ICSE](https://github.com/criszy/Troc) 23]
- [Adaptive Performance Anomaly Detection for Online Service Systems via Pattern Sketching](http://arxiv.org/abs/2201.02944) [ICSE 22]

### Benchmark

-  DBPA: A Benchmark for Transactional Database Performance Anomalies  [SIGMOD 23]


## Testing

### Concurrency Testing

- [Race Directed Random Testing of Concurrent Programs]( https://dl.acm.org/doi/10.1145/1375581.1375584 ) [PLDI 08]
- [Sound and Efficient Concurrency Bug Prediction](  https://dl.acm.org/doi/10.1145/3468264.3468549 ) [ESEC/FSE 21]
- [How are distributed bugs diagnosed and fixed through system logs?](https://linkinghub.elsevier.com/retrieve/pii/S0950584919302496) [Information and Software Technology 20]

### Fuzzing

- [Krace: Data Race Fuzzing for Kernel File Systems](https://ieeexplore.ieee.org/document/9152693/) [SP 20]

### Root Cause Analyze

- [BALANCE: Bayesian Linear Attribution for Root Cause Localization](http://arxiv.org/abs/2301.13572) [SIGMOD 23]
- [Towards Effective Bug Triage with Software Data Reduction Techniques](https://ieeexplore.ieee.org/document/6815966/) [TKDE 15]

### Fault Location

- [Effective fault localization and context‐aware debugging for concurrent programs](https://onlinelibrary.wiley.com/doi/10.1002/stvr.1797) [Softw Test Verif Reliab 22]
- [Fault Localization with Code Coverage Representation Learning](https://dl.acm.org/doi/10.1109/ICSE43902.2021.00067) [ICSE 21]
