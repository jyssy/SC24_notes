## Workflow optimization B309

### LLM performance tools
- - LLM Pilot perf predictions
- - have reduxed the over spend by more than 2X
- - - eveloped LLM pilot
- - - investigated  what factors impact the inference performance
- - - good performance model
- - - have open sourced the projects

1. [fmperf](https://github.com/fmperf-project/fmperf)

2. [LLM-performance-prediction](https://github.com/IBM/LLM-performance-prediction)

- - files for this presentation in [workflows](workflows)

### DFTracer
- - [Paper: DFTracer: An Analysis-Friendly Data Flow Tracer for AI-Driven Workflows](https://doi.org/10.1109/SC41406.2024.000)
- - [open sourced the project, Read the Docs](https://dftracer.readthedocs.io/en/latest/#)
- - [Github](https://github.com/hariharan-devarajan/dftracer)
- - Deep learning workflows
- -  billions of IO events on so many data formats
Main causes: 

1. turning C typees intop python types
2. lack of parallel ...

- - async/IO challenges
- - analysis ready
- - uses [JSON lines](https://jsonlines.org/)
- - - portables; derived using chrometracing format
- - comments about python being more expensive than C
- - files in [dftracer](dftracer)

### Efficient weighted graph matching on GPUs

- - [paper](https://doi.org/10.1109/SC41406.2024.000)
- - Pacific Northwest National Laboratory
- - articles about runtime
- - - [What is runtime?](https://www.techtarget.com/searchsoftwarequality/definition/runtime)
- - - 