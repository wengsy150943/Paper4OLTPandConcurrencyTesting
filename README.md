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
- [Coo: Consistency Check for Transactional Databases](http://arxiv.org/abs/2206.14602)

## OLTP

### Implementation

- [GeoGauss: Strongly Consistent Coordinator-Free OLTP for Geo-Replicated SQL Database](https://dl.acm.org/doi/abs/10.1145/3588916)  [SIGMOD 23]
- [P4DB - The Case for In-Network OLTP]( https://doi.org/10.1145/3514221.3517825 ) [SIGMOD 22]
- [GaccO - A GPU-accelerated OLTP DBMS ]( https://doi.org/10.1145/3514221.3517876 )[SIGMOD 22]
- [Proteus: Autonomous Adaptive Storage for Mixed Workloads]( https://doi.org/10.1145/3514221.3517834 ) [SIGMOD 22]

### Concurrency Control

-  [Polaris: Enabling Transaction Priority in Optimistic Concurrency Control](https://dl.acm.org/doi/abs/10.1145/3588724) [SIGMOD 23]
- [Diva: Making MVCC Systems HTAP-Friendly]( https://doi.org/10.1145/3514221.3526135 ) [SIGMOD 22]
- [Plor: General Transactions with Predictable, Low Tail Latency]( https://doi.org/10.1145/3514221.3517879 ) [SIGMOD 22]
- [Strictly Serializable Timestamp Ordering by Avoiding the Timestamp-Inversion Pitfall](https://arxiv.org/abs/2305.14270) [OSDI 23]
- [Polyjuice: High-Performance Transactions via Learned Concurrency Control](https://www.usenix.org/conference/osdi21/presentation/wang-jiachen) [OSDI 21]
- Verifying vMVCC, a high-performance database using multi-version concurrency control [OSDI]
- [Contention-aware lock scheduling for transactional databases](http://dl.acm.org/citation.cfm?doid=3187009.3177740) [VLDB 18]
- [Cornus: atomic commit for a cloud DBMS with storage disaggregation](https://dl.acm.org/doi/10.14778/3565816.3565837) [VLDB 22]
- [Making Cache Monotonic and Consistent](https://www.vldb.org/pvldb/vol16/p891-cao.pdf) [VLDB 22]
- [Scalable and Robust Snapshot Isolation for High-Performance Storage Engines](https://dl.acm.org/doi/10.14778/3583140.3583157) [VLDB 22]

### Transaction

-  [Transaction Scheduling: From Conflicts to Runtime Conflicts](https://dl.acm.org/doi/abs/10.1145/3588706) [SIGMOD 23]
-  [Towards a Practical Database Management System with Verifiable ACID Properties and Transaction Correctness]( https://doi.org/10.1145/3514221.3517851 ) [SIGMOD 22]
-  [Skeena: Efficient and Consistent Cross-Engine Transactions]( https://doi.org/10.1145/3514221.3526171 ) [SIGMOD 22]
-  [Natto: Providing Distributed Transaction Prioritization for High-Contention Workloads]( https://doi.org/10.1145/3514221.3526161 ) [SIGMOD 22]
-  [Fine-Grained Re-Execution for Efficient Batched Commit of Distributed Transactions](https://www.vldb.org/pvldb/vol16/p1930-dong.pdf) [VLDB 22]

### Anomaly Detection

-  [Robust and Transferable Log-based Anomaly Detection](http://arxiv.org/abs/2102.11570)   [SIGMOD 23] 
- [Detecting Isolation Bugs via Transaction Oracle Construction]( https://doi.org/10.5281/zenodo.7645649 ) [ [ICSE](https://github.com/criszy/Troc) 23]
- [Adaptive Performance Anomaly Detection for Online Service Systems via Pattern Sketching](http://arxiv.org/abs/2201.02944) [ICSE 22]

### Benchmark

-  [DBPA: A Benchmark for Transactional Database Performance Anomalies](https://dl.acm.org/doi/abs/10.1145/3588926)  [SIGMOD 23]
-  [Scientific benchmarking of parallel computing systems: twelve ways to tell the masses when reporting performance results](https://dl.acm.org/doi/10.1145/2807591.2807644) [SC15]
-  [VeriBench: Analyzing the Performance of Database Systems with Verifiability](https://dl.acm.org/doi/10.14778/3598581.3598588) [VLDB 22]


## Testing

### Concurrency Testing

- [Race Directed Random Testing of Concurrent Programs]( https://dl.acm.org/doi/10.1145/1375581.1375584 ) [PLDI 08]
- [Sound and Efficient Concurrency Bug Prediction](  https://dl.acm.org/doi/10.1145/3468264.3468549 ) [ESEC/FSE 21]
- [How are distributed bugs diagnosed and fixed through system logs?](https://linkinghub.elsevier.com/retrieve/pii/S0950584919302496) [Information and Software Technology 20]
- [Demystifying and Checking Silent Semantic Violations in Large Distributed Systems](https://www.usenix.org/system/files/osdi22-lou-demystifying.pdf) [OSDI 22]
- [Automatic Reliability Testing for Cluster Management Controllers](https://www.usenix.org/system/files/osdi22-sun.pdf) [OSDI 22]

### Fuzzing

- [Krace: Data Race Fuzzing for Kernel File Systems](https://ieeexplore.ieee.org/document/9152693/) [SP 20]
- [DynSQL: Stateful Fuzzing for Database Management Systems with Complex and Valid SQL Query Generation](https://www.usenix.org/system/files/sec23summer_60-jiang_zu_ming-prepub.pdf) [Security 23]
- [Griffin : Grammar-Free DBMS Fuzzing](https://dl.acm.org/doi/abs/10.1145/3551349.3560431) [ASE 22]

### Root Cause Analyze

- [BALANCE: Bayesian Linear Attribution for Root Cause Localization](http://arxiv.org/abs/2301.13572) [SIGMOD 23]
- [Towards Effective Bug Triage with Software Data Reduction Techniques](https://ieeexplore.ieee.org/document/6815966/) [TKDE 15]
- Relational Debugging --- Pinpointing Root Causes of Performance Problems [OSDI 23]

### Fault Location

- [Effective fault localization and context‐aware debugging for concurrent programs](https://onlinelibrary.wiley.com/doi/10.1002/stvr.1797) [Softw Test Verif Reliab 22]
- [Fault Localization with Code Coverage Representation Learning](https://dl.acm.org/doi/10.1109/ICSE43902.2021.00067) [ICSE 21]
