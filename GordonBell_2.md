## Gordon Bell award presentatoins, session # 2

### MProt-DPO: Breaking the ExaFLOPS Barrier for Multimodal Protein Design Workflows with Direct Preference Optimization

- https://www.anl.gov/article/argonne-team-breaks-new-ground-in-aidriven-protein-design

`“Demonstrating that this approach delivers strong scientific results at extreme scales is an important step toward building more robust AI models. It also moves us closer to autonomous discovery, where AI can help streamline not only experiments but the entire scientific process.” — Arvind Ramanathan, Argonne computational biologist`

- https://sc24.conference-program.com/presentation/?id=gb101&sess=sess497

#### Description

`We present a scalable, end-to-end workflow for protein design. By augmenting protein sequences with natural language descriptions of biochemical properties, we train generative models to preferentially align with protein fitness landscapes. Through complex experimental- and simulation-based observations, we integrate these measures as preferred parameters for generating new protein variants and demonstrate our workflow on five diverse supercomputers. We achieve >1 ExaFLOPS sustained performance in mixed precision on each supercomputer and a maximum sustained performance of 4.11 ExaFLOPS and peak performance of 5.57 ExaFLOPS. We establish the performance of our model on two tasks: (1) across a predetermined benchmark dataset of deep mutational scanning experiments to optimize the fitness-determining mutations in the yeast protein HIS7, and (2) in optimizing the design of the enzyme malate dehydrogenase to achieve lower activation barriers (and therefore increased catalytic rates) using simulation data. Our implementation thus sets high watermarks for multimodal protein design workflows.`

### Breaking the Molecular Dynamics Timescale Barrier Using a Wafer-Scale System

- https://sc24.conference-program.com/presentation/?id=gb104&sess=sess497

#### Description

`Molecular dynamics (MD) simulations have transformed our understanding of the nanoscale, driving breakthroughs in materials science, computational chemistry, and several other fields, including biophysics and drug design. Even on exascale supercomputers, however, runtimes are excessive for systems and timescales of scientific interest. Here, we demonstrate strong scaling of MD simulations on the Cerebras Wafer Scale Engine. By dedicating a processor core for each simulated atom, we demonstrate a 457-fold improvement in timesteps per second versus the Frontier GPU-based exascale platform, along with a large improvement in timesteps per unit energy. Reducing every year of runtime to less than a day unlocks currently inaccessible timescales of slow microstructure transformation processes that are critical for understanding material behavior and function. Our dataflow algorithm runs embedded-atom method (EAM) simulations at rates over 699k timesteps per second for problems with up to 800k atoms. This demonstrated performance is unprecedented for general-purpose processing cores.`

### Breaking the Million-Electron and 1 EFLOP/s Barriers: Biomolecular-Scale Ab Initio Molecular Dynamics Using MP2 Potentials

- https://sc24.conference-program.com/presentation/?id=gb106&sess=sess497

#### Description

`The accurate simulation of complex biochemical phenomena has historically been hampered by the computational requirements of high-fidelity molecular-modeling techniques. Quantum mechanical methods, such as \emph{ab initio} wave-function (WF) theory, deliver the desired accuracy, but have impractical scaling for modeling biosystems with thousands of atoms. Combining molecular fragmentation with MP2 perturbation theory, this study presents an innovative approach that enables biomolecular-scale \emph{ab initio} molecular dynamics (AIMD) simulations at WF theory level. Leveraging the resolution-of-the-identity approximation for Hartree-Fock and MP2 gradients, our approach eliminates computationally intensive four-center integrals and their gradients, while achieving near-peak performance on modern GPU architectures. The introduction of asynchronous time steps minimizes time step latency, overlapping computational phases and effectively mitigating load imbalances. Utilizing up to 9,400 nodes of Frontier and achieving 59% (1006.7 PFLOP/s) of its double-precision floating-point peak, our method enables us to break the million-electron and 1 EFLOP/s barriers for AIMD simulations with quantum accuracy.`
