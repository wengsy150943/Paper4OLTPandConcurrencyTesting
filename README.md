# Paper4OLTPandConcurrencyTesting

This repository lists papers with topics covering OLTP and error testing (especially concurrency-related testing).

New PR is welcome for any material that you think should be included in this collection. .

If you want to add new paper, please follow link format:

```markdown
paperName(with access link) [MeetingName(with open source code, if exists) Year]
```

[TOC]

## Survey and Tutorial

- [10 Years of research on debugging concurrent and multicore software: a systematic mapping study](http://link.springer.com/10.1007/s11219-015-9301-7) [Software Quality Journal 17]
- [Coo: Consistency Check for Transactional Databases](http://arxiv.org/abs/2206.14602)
- [Techniques and Efficiencies from Building a Real-Time DBMS](https://www.vldb.org/pvldb/vol16/p3676-srinivasan.pdf) [VLDB 23]
- [LLM for Data Management](https://dbgroup.cs.tsinghua.edu.cn/ligl/papers/p2031-li-vldb2024.pdf) [VLDB 24]
- [Native Distributed Databases: Problems, Challenges and Opportunities](https://www.vldb.org/pvldb/vol17/p4217-xu.pdf) [VLDB 24]

## OLTP

### Implementation

- [GeoGauss: Strongly Consistent Coordinator-Free OLTP for Geo-Replicated SQL Database](https://dl.acm.org/doi/abs/10.1145/3588916) [SIGMOD 23]
- [P4DB - The Case for In-Network OLTP](https://doi.org/10.1145/3514221.3517825) [SIGMOD 22]
- [GaccO - A GPU-accelerated OLTP DBMS ](https://doi.org/10.1145/3514221.3517876)[SIGMOD 22]
- [Proteus: Autonomous Adaptive Storage for Mixed Workloads](https://doi.org/10.1145/3514221.3517834) [SIGMOD 22]
- [Progressive Partitioning for Parallelized Query Execution in Google's Napa](https://www.vldb.org/pvldb/vol16/p3475-sankaranarayanan.pdf) [VLDB 23]
- [Krypton: Real-time Serving and Analytical SQL Engine at ByteDance](https://www.vldb.org/pvldb/vol16/p3528-chen.pdf) [VLDB 23]
- [OceanBase Paetica: A Hybrid Shared-nothing/Shared-everything Database for Supporting Single Machine and Distributed Cluster](https://www.vldb.org/pvldb/vol16/p3728-xu.pdf) [VLDB 23]
- [PolarDB-SCC: A Cloud-Native Database Ensuring Low Latency for Strongly Consistent Reads](https://www.vldb.org/pvldb/vol16/p3754-chen.pdf) [VLDB 23]
- [Natural Language Interfaces for Databases with Deep Learning](https://www.vldb.org/pvldb/vol16/p3878-katsogiannis-meimarakis.pdf) [VLDB 23]
- [TiQuE: Improving the Transactional Performance of Analytical Systems for True Hybrid Workloads](https://www.vldb.org/pvldb/vol16/p2274-faria.pdf) [VLDB 23]
- [The art of latency hiding in modern database engines](https://dl.acm.org/doi/10.14778/3632093.3632117) [VLDB 23]
- [CoroBase: coroutine-oriented main-memory database engine](https://dl.acm.org/doi/10.14778/3430915.3430932) [VLDB 21]
- [ScaleDB: A Scalable, Asynchronous In-Memory Database](https://www.usenix.org/conference/osdi23/presentation/mehdi) [OSDI 23]
- [NOMAD: Non-Exclusive Memory Tiering via Transactional Page Migration](https://www.usenix.org/system/files/osdi24-xiang.pdf) [OSDI 24]
- [DRust: Language-Guided Distributed Shared Memory with Fine Granularity, Full Transparency, and Ultra Efficiency](https://www.usenix.org/system/files/osdi24-ma-haoran.pdf) [OSDI 24]
- [GaussDB: A Cloud-Native Multi-Primary Database with Compute-Memory-Storage Disaggregation](https://www.vldb.org/pvldb/vol17/p3786-li.pdf) [VLDB 24]
- [TDSQL: Tencent Distributed Database System](https://www.vldb.org/pvldb/vol17/p3869-chen.pdf) [VLDB 24]
- [LazyLog: A New Shared Log Abstraction for Low-Latency Applications](https://doi.org/10.1145/3694715.3695983) [[SOSP](https://github.com/dassl-uiuc/LazyLog-Artifact) 24]

### Storage

- [What Modern NVMe Storage Can Do, And How To Exploit It: High-Performance I/O for High-Performance Storage Engines](https://www.vldb.org/pvldb/vol16/p2090-haas.pdf) [VLDB 23]
- [NVM: Is it Not Very Meaningful for Databases?](https://www.vldb.org/pvldb/vol16/p2444-koutsoukos.pdf) [VLDB 23]
- [An Empirical Evaluation of Columnar Storage Formats](https://www.vldb.org/pvldb/vol17/p148-zeng.pdf) [VLDB 23]
- [Understanding the Performance Implications of the Design Principles in Storage-Disaggregated Databases](https://dl.acm.org/doi/pdf/10.1145/3654983) [SIGMOD 24]
- [Structural Designs Meet Optimality: Exploring Optimized LSM-tree Structures in A Colossal Configuration Space](https://dl.acm.org/doi/pdf/10.1145/3654978) [SIGMOD 24]
- [CaaS-LSM: Compaction-as-a-Service for LSM-based Key-Value Stores in Storage Disaggregated Infrastructure](https://dl.acm.org/doi/pdf/10.1145/3654927) [[SIGMOD](https://github.com/asu-idi/CaaS-LSM) 24]
- [LavaStore: ByteDance’s Purpose-built, High-performance, Cost-effective Local Storage Engine for Cloud Services](https://www.vldb.org/pvldb/vol17/p3799-jiao.pdf) [VLDB 24]
- [LeanStore: A High-Performance Storage Engine for NVMe SSDs](https://www.vldb.org/pvldb/vol17/p4536-leis.pdf) [VLDB 24]
- [PALF: Replicated Write-Ahead Logging for Distributed Databases](https://www.vldb.org/pvldb/vol17/p3745-xu.pdf) [[VLDB](https://github.com/oceanbase/oceanbase/tree/develop/src/logservice/palf) 24]

### Concurrency Control

- [Polaris: Enabling Transaction Priority in Optimistic Concurrency Control](https://dl.acm.org/doi/abs/10.1145/3588724) [SIGMOD 23]
- [Diva: Making MVCC Systems HTAP-Friendly](https://doi.org/10.1145/3514221.3526135) [SIGMOD 22]
- [Plor: General Transactions with Predictable, Low Tail Latency](https://doi.org/10.1145/3514221.3517879) [SIGMOD 22]
- [Strictly Serializable Timestamp Ordering by Avoiding the Timestamp-Inversion Pitfall](https://arxiv.org/abs/2305.14270) [OSDI 23]
- [Polyjuice: High-Performance Transactions via Learned Concurrency Control](https://www.usenix.org/conference/osdi21/presentation/wang-jiachen) [OSDI 21]
- [Verifying vMVCC, a high-performance database using multi-version concurrency control](https://www.usenix.org/system/files/osdi23-chang.pdf) [OSDI 23]
- [Contention-aware lock scheduling for transactional databases](http://dl.acm.org/citation.cfm?doid=3187009.3177740) [VLDB 18]
- [Cornus: atomic commit for a cloud DBMS with storage disaggregation](https://dl.acm.org/doi/10.14778/3565816.3565837) [VLDB 22]
- [Making Cache Monotonic and Consistent](https://www.vldb.org/pvldb/vol16/p891-cao.pdf) [VLDB 22]
- [Scalable and Robust Snapshot Isolation for High-Performance Storage Engines](https://dl.acm.org/doi/10.14778/3583140.3583157) [VLDB 22]
- [OptiQL: Robust Optimistic Locking for Memory-Optimized Indexes](https://www2.cs.sfu.ca/~tzwang/optiql.pdf) [[SIGMOD](https://github.com/sfu-dis/optiql)24]
- [A study of database performance sensitivity to experiment settings](https://dl.acm.org/doi/10.14778/3523210.3523221) [VLDB 22]
- [An evaluation of distributed concurrency control](https://dl.acm.org/doi/10.14778/3055540.3055548) [VLDB 17]
- [NCC: Natural Concurrency Control for Strictly Serializable Datastores by Avoiding the Timestamp-Inversion Pitfall](https://www.usenix.org/conference/osdi23/presentation/lu) [OSDI 23]
- [Motor: Enabling Multi-Versioning for Distributed Transactions on Disaggregated Memory](https://www.usenix.org/system/files/osdi24-zhang-ming.pdf) [OSDI 24]
- [Massively Parallel Multi-Versioned Transaction Processing](https://www.usenix.org/system/files/osdi24-qian.pdf) [OSDI 24]
- [Towards Optimal Transaction Scheduling](https://dl.acm.org/doi/10.14778/3681954.3681956) [[VLDB](https://github.com/audreyccheng/transaction-scheduling) 24]

### Transaction
- [FC: Adaptive Atomic Commit via Failure Detection](https://ieeexplore.ieee.org/document/10597727) [ICDE 24]
- [LCL: A Lock Chain Length-based Distributed  Algorithm for Deadlock Detection and Resolution](https://ieeexplore.ieee.org/document/10184686) [ICDE 23]
- [Transaction Scheduling: From Conflicts to Runtime Conflicts](https://dl.acm.org/doi/abs/10.1145/3588706) [SIGMOD 23]
- [Towards a Practical Database Management System with Verifiable ACID Properties and Transaction Correctness](https://doi.org/10.1145/3514221.3517851) [SIGMOD 22]
- [Skeena: Efficient and Consistent Cross-Engine Transactions](https://doi.org/10.1145/3514221.3526171) [SIGMOD 22]
- [Natto: Providing Distributed Transaction Prioritization for High-Contention Workloads](https://doi.org/10.1145/3514221.3526161) [SIGMOD 22]
- [Fine-Grained Re-Execution for Efficient Batched Commit of Distributed Transactions](https://www.vldb.org/pvldb/vol16/p1930-dong.pdf) [VLDB 23]
- [Epoxy: ACID Transactions Across Diverse Data Stores](https://www.vldb.org/pvldb/vol16/p2742-kraft.pdf) [VLDB 23]
- [Epoch-based Commit and Replication in Distributed OLTP Databases](https://www.vldb.org/pvldb/vol14/p743-lu.pdf) [VLDB 21]
- [Efficient Distributed Transaction Processing in Heterogeneous Networks](https://www.vldb.org/pvldb/vol16/p1372-lu.pdf) [VLDB 23]
- [NOC-NOC: Towards Performance-optimal Distributed Transactions](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/665216/main.pdf?sequence=1) [SIGMOD 24]
- [Chardonnay: Fast and General Datacenter Transactions for On-Disk Databases](https://www.usenix.org/conference/osdi23/presentation/eldeeb) [OSDI 23]
- [Opportunities for optimism in contended main-memory multicore transactions](https://link.springer.com/10.1007/s00778-021-00719-9) [VLDB 22]
- [Unifying Timestamp with Transaction Ordering for MVCC with Decentralized Scalar Timestamp](https://www.usenix.org/conference/nsdi21/presentation/wei) [NSDI 21]
- [Knock Out 2PC with Practicality Intact: a High-performance and General Distributed Transaction Protocol](https://arxiv.org/pdf/2302.12517) [ICDE 23]
- [Lion: Minimizing Distributed Transactions through Adaptive Replica Provision](https://arxiv.org/pdf/2403.11221) [ICDE 24]

### Anomaly Detection

- [Robust and Transferable Log-based Anomaly Detection](http://arxiv.org/abs/2102.11570) [SIGMOD 23]
- [Detecting Isolation Bugs via Transaction Oracle Construction](https://doi.org/10.5281/zenodo.7645649) [ [ICSE](https://github.com/criszy/Troc) 23]
- [Adaptive Performance Anomaly Detection for Online Service Systems via Pattern Sketching](http://arxiv.org/abs/2201.02944) [ICSE 22]
- [IsoVista: Black-box Checking Database Isolation Guarantees](https://www.vldb.org/pvldb/vol17/p4325-liu.pdf) [[VLDB](https://github.com/hengxin/IsoVista) 24]

### Benchmark

- [DBPA: A Benchmark for Transactional Database Performance Anomalies](https://dl.acm.org/doi/abs/10.1145/3588926) [SIGMOD 23]
- [Scientific benchmarking of parallel computing systems: twelve ways to tell the masses when reporting performance results](https://dl.acm.org/doi/10.1145/2807591.2807644) [SC 15]
- [VeriBench: Analyzing the Performance of Database Systems with Verifiability](https://dl.acm.org/doi/10.14778/3598581.3598588) [VLDB 22]
- [CDSBen: Benchmarking the Performance of Storage Services in Cloud-native Database System at ByteDance](https://www.vldb.org/pvldb/vol16/p3584-tang.pdf) [VLDB 23]
- [Leopard: A Black-Box Approach for Efficiently Verifying Various Isolation Levels](https://ieeexplore.ieee.org/abstract/document/10184872) [ICDE 23]
- [DB-MAGS: Multi-Anomaly Data Generation System for Transactional Databases](https://www.vldb.org/pvldb/vol17/p4497-shen.pdf) [[VLDB](https://github.com/qifeng1128/DB-MAGS) 24]

## Testing

### Concurrency Testing

- [Race Directed Random Testing of Concurrent Programs](https://dl.acm.org/doi/10.1145/1375581.1375584) [PLDI 08]
- [Sound and Efficient Concurrency Bug Prediction](https://dl.acm.org/doi/10.1145/3468264.3468549) [ESEC/FSE 21]
- [How are distributed bugs diagnosed and fixed through system logs?](https://linkinghub.elsevier.com/retrieve/pii/S0950584919302496) [Information and Software Technology 20]
- [Demystifying and Checking Silent Semantic Violations in Large Distributed Systems](https://www.usenix.org/system/files/osdi22-lou-demystifying.pdf) [OSDI 22]
- [Automatic Reliability Testing for Cluster Management Controllers](https://www.usenix.org/system/files/osdi22-sun.pdf) [OSDI 22]
- [R^3: Record-Replay-Retroaction for Database-Backed Applications](https://www.vldb.org/pvldb/vol16/p3085-li.pdf) [VLDB 23]
- [LST-Meter: Benchmarking Log-Structured Tables in the Cloud](https://arxiv.org/pdf/2305.01120.pdf) [SIGMOD 24]
- [Detecting Transactional Bugs in Database Engines via Graph-Based Oracle Construction](https://www.usenix.org/system/files/osdi23-jiang.pdf) [[OSDI](https://github.com/JZuming/TxCheck) 23]
- [Differentially testing database transactions for fun and profit](http://tcse.cn/~wsdou/papers/2022-issta-grand.pdf) [[ISSTA](https://github.com/tcse-iscas/Grand) 22]
- [Ozz: identifying kernel out-of-order concurrency bugs with In-vivo memory access reordering](https://gts3.org/assets/papers/2024/jeong:ozz.pdf) [[SOSP](https://github.com/casys-kaist/ozz) 24]

### Fuzzing

- [Krace: Data Race Fuzzing for Kernel File Systems](https://ieeexplore.ieee.org/document/9152693/) [SP 20]
- [DynSQL: Stateful Fuzzing for Database Management Systems with Complex and Valid SQL Query Generation](https://www.usenix.org/system/files/sec23summer_60-jiang_zu_ming-prepub.pdf) [Security 23]
- [Griffin : Grammar-Free DBMS Fuzzing](https://dl.acm.org/doi/abs/10.1145/3551349.3560431) [ASE 22]
- [Unicorn: detect runtime errors in time-series databases with hybrid input synthesis](https://dl.acm.org/doi/10.1145/3533767.3534364) [ISSTA 23]
- [PINOLO: Detecting Logical Bugs in Database Management Systems with Approximate Query Synthesis](https://www.usenix.org/system/files/atc23-hao.pdf) [ATC 23]
- [The Use of Likely Invariants as Feedback for Fuzzers](https://www.usenix.org/system/files/sec21-fioraldi.pdf) [SEC 21]
- [Semantic fuzzing with zest](https://dl.acm.org/doi/10.1145/3293882.3330576) [ISSTA 19]
- [SQLaser: detecting DBMS logic bugs with clause-guided fuzzing](http://arxiv.org/abs/2407.04294) preprint
- [Blackbox fuzzing of distributed systems with multi-dimensional inputs and symmetry-based feedback pruning](https://dx.doi.org/10.14722/ndss.2025.241912) [[NDSS](https://dx.doi.org/10.14722/ndss.2025.241912) 25]

### Other Testing Methods

- [Detecting logic bugs in database engines via equivalent expression transformation](https://jzuming.github.io/paper/osdi24-jiang.pdf) [[OSDI](https://github.com/JZuming/EET) 24]
- [Detecting metadata-related logic bugs in database systems via raw database construction](https://doi.org/10.14778/3659437.3659445) [VLDB 24]
- [Keep it simple: testing databases via differential query plans](https://bajinsheng.github.io/assets/pdf/dqp_sigmod24.pdf) [[SIGMOD](https://github.com/sqlancer/sqlancer/issues/918) 24]
- [Detecting optimization bugs in database engines via non-optimizing reference engine construction](https://doi.org/10.1145/3368089.3409710) [FSE 20]
- [Testing Database Engines via Query Plan Guidance](https://arxiv.org/pdf/2312.17510.pdf) [[ICSE](https://github.com/sqlancer/sqlancer/issues/641) 23]
- [Testing Database Engines via Pivoted Query Synthesis](https://www.usenix.org/system/files/osdi20-rigger.pdf) [[OSDI](https://www.usenix.org/conference/osdi20/presentation/rigger) 20]
- [Detecting Optimization Bugs in Database Engines via Non-Optimizing Reference Engine Construction](https://dl.acm.org/doi/pdf/10.1145/3368089.3409710) [FSE 20]
- [When Amnesia Strikes: Understanding and Reproducing Data Loss Bugs with Fault Injection](https://dl.acm.org/doi/10.14778/3681954.3681980) [[VLDB](https://github.com/dsrhaslab/lazyfs) 24]
- [Efficient Reproduction of Fault-Induced Failures in Distributed Systems with Feedback-Driven Fault Injection](https://doi.org/10.1145/3694715.3695979) [[SOSP](https://github.com/OrderLab/Anduril) 24]
- [Understanding and Reusing Test Suites Across Database Systems](https://doi.org/10.1145/3698829) [SIGMOD 24]

### Root Cause Analyze

- [BALANCE: Bayesian Linear Attribution for Root Cause Localization](http://arxiv.org/abs/2301.13572) [SIGMOD 23]
- [Towards Effective Bug Triage with Software Data Reduction Techniques](https://ieeexplore.ieee.org/document/6815966/) [TKDE 15]
- [Relational Debugging --- Pinpointing Root Causes of Performance Problems](https://www.usenix.org/system/files/osdi23-ren.pdf) [[OSDI](https://gitlab.dsrg.utoronto.ca/dsrg/perspect) 23]

### Fault Location

- [Effective fault localization and context‐aware debugging for concurrent programs](https://onlinelibrary.wiley.com/doi/10.1002/stvr.1797) [Softw Test Verif Reliab 22]
- [Fault Localization with Code Coverage Representation Learning](https://dl.acm.org/doi/10.1109/ICSE43902.2021.00067) [ICSE 21]

### Distributed System Testing

- [Greybox Fuzzing of Distributed Systems](https://dl.acm.org/doi/10.1145/3576915.3623097) [CCS 23]
- [An Analysis of Network-Partitioning Failures in Cloud Systems](https://www.usenix.org/conference/osdi18/presentation/alquraan) [OSDI 18]
- [Why Is Random Testing Effective for Partition Tolerance Bugs?](https://dl.acm.org/doi/10.1145/3158134) [POPL 17]

## Other Paper List with similar topics

- [Recent Fuzzing Paper](https://wcventure.github.io/FuzzingPaper/)
- [AP Paper](https://github.com/Wind-Gone/OLAP-Paper)
- [AI4DB Paper](https://github.com/Wind-Gone/Ai4DB-Paper)
- [LLM4DB Paper](https://github.com/code4DB/LLM4DB)
- [Awesome Database Learning](https://github.com/pingcap/awesome-database-learning)
- [Readings in Database Systems](http://www.redbook.io/all-readings.html)
