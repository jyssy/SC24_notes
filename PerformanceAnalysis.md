## Presentations

1:30pm - 2pm EST

### Versatile Datapath Soft Error Detection on the Cheap for HPC Applications

- - https://sc24.conference-program.com/presentation/?id=pap454&sess=sess379
    AuthorsYafan Huang
    Sheng Di
    Zhaorui Zhang
    Xiaoyi Lu
    Guanpeng Li

[paper](https://doi.org/10.1109/SC41406.2024.000)

### Abstract

`With the ongoing reduction in technology sizes and voltage levels, modern microprocessors are increasingly susceptible to soft errors, corrupting datapath units during program execution. While these error types have received considerable attention recently, existing solutions either confine themselves to limited scopes or incur massive overheads in performance and power consumption, hindering practical usage. In this work, we propose CONDA, a novel error detection technique based on code transformation and static program analysis, achieving versatile datapath protection at low cost. At compile time, CONDA analyzes program characteristics and transforms the original program code without complicating its control-flow and memory access patterns. At runtime, CONDA detects datapath errors with low overhead and latency. The evaluation of 38 benchmarks and a parallel HPC simulation reveals that ConDa only incurs 57.79% runtime overhead, which is 41.84% faster than existing state-of-the-art, with the same level of error detection effectiveness and low detection latency.`

- - soft errors
- - the soft error can cascade
- - hardware errors, but expensive to detect
- - memory errors are easier to detect. but data path errors are much more expensive to detect
- - could cause a faulty jump, instead of the intended path
- - SWIFT and gZDC have large runtime overheads

1. defect 1 : complicated program control flow
2. defect 2 : frequent memory access

- - Goal is to provide robust entire datapath protection with low runtime overheard
- - should be plug and play
- - suggests ConDa
- - lazy checking motion
- - using duplicate instruction to detect data-flow errors
- - designed a signature to operate with a block as a unique thing
- - also buffering into one register
- - ConDa: adaptive detection placement

2pm - 2:30pm EST

### MCBound: an Online Framework to Characterize and Classify Memory/Compute-bound HPC Jobs

- - https://sc24.conference-program.com/presentation/?id=pap563&sess=sess379
- - DOI: 10.1109/SC41406.2024.00062

AuthorsFrancesco Antici
Andrea Bartolini
Zeynep Kiziltan
Ozalp Babaoglu
Yuetsu Kodama
2:30pm - 3pm EST
GVARP: Detecting Performance Variance on Large-Scale Heterogeneous System

### Abstract

`Modern High-Performance Computing (HPC) systems play a fundamental role in driving scientific research, as they execute computationally intensive jobs originating from diverse domains. However, HPC jobs are characterized by conflicting computational requirements, which may cause inefficiencies in resource usage, system throughput and energy consumption. One approach to tackling this problem is to distinguish between memory-bound and compute-bound jobs at their submission time, with the goal of making informed decisions about their execution. In this paper, we present MCBound, the first online data-driven framework to classify HPC jobs as memory/compute-bound before job execution, without user intervention. We propose a systematic characterization technique to generate a reference dataset from historical data for initial classification model training. Using the proposed characterization technique, we analyze the data of 2.2 million job runs on the Supercomputer Fugaku1, a production HPC system installed at the RIKEN Center for Computational Science, in Japan. We implement MCBound for Fugaku and classify the jobs executed during February 2024. Our approach is proven effective, as it obtains an F1-macro average score of at least 0.89 as prediction quality, while incurring a negligible overhead on the system’s operations. Our Python-based implementation of MCBound can be seamlessly configured and deployed in other HPC systems.`

- - paper in the [perf_analysis folder](perf_analysis/SC24__MCBound_Framework.pdf)
