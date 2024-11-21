## notes for python 24 demo workshop - 11-18-2024

== https://hppss.github.io/SC24/index.html#

- papers: https://hppss.github.io/SC24/papers.html

Repo of [images](python_demo) from the Python workshop

### Dask

- https://www.dask.org/
- make things visual, people like dashboards
- dashboards help respresent cost analysis to show that scaling is not expensive at at scale
- $ pip install dask
- make dask useful and easy on a laptop
- does not have to work on a remote system
- Could cuda be better run on a local laptop so more people would be able to start using it
- for some reason, some sysadmins did not want dask to run on their HPCs
- people could also run dask on kubernetesm but also on yarn etc
- to run on bigger machines, things would need to be better described and also need more node pools
- their cloud accounts, using django to start up and run these
- Dask arrays, sort of like NumPy, but promotes a library called Blaze https://blaze.pydata.org/
- The Blaze Ecosystem: https://blaze.pydata.org/
- uses COILED
- use APIs
- matthewrocklin.com
- files in [dask](dask)

### Coiled

- https://www.coiled.io/
- also reinvigorated SLURM arrays

### DynD

- https://github.com/libdynd/dynd-python

### Arkouda

- https://github.com/Bears-R-Us (Bears R Us GitHub repo a the high level)
- https://pypi.org/project/arkouda/
- https://pypi.org/project/arkouda/
- arkouda client written in python
- the ideais that we need to scale python to work in the cloud
- install arkouda: https://bears-r-us.github.io/arkouda/setup/install_menu.html
- docker containers: https://hub.docker.com/r/hokiegeek2/arkouda-server?
- if you can write numpy code, you can write arkouda code
- More than NumPY for HPC
- written in Chapel
- files in [arkouda](arkouda)

### CUDA Python Object Models and Parallelism Models

#### CUDA Python Object Models and Parallelism Models - Andy Terrel

- https://github.com/Roman-Supernova-PIT/phrosty
- CuPy is a near 1:1 map to NumPY CuPy
- NumPy & SciPy for GPU
- [website](https://cupy.dev/)
- https://github.com/cupy/cupy
- uses nvmath-oython: https://github.com/NVIDIA/nvmath-python
- attempted to use with grace hopper architecture
- cupyx (need to look up how this differs from cupy proper)
- NVIDIA Future of Computing: https://github.com/NVIDIA/accelerated-computing-hub
- files in [cupy_nvmath](cupy_nvmath)

### Seamlessly scale your python program from single CPU core to multi-GPU multi-node HPC cluster with cuNumeric - Wonchan Lee, Manolis Papadakis, Mike Bauer, Bo Dong

-

### Various notes and comments

- Dragon for HPC
- https://dragonhpc.org/portal/index.html
- https://github.com/DragonHPC/dragon
