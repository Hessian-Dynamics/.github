# Hessian Dynamics

I am building open-source infrastructure for computational chemistry and molecular simulations. 

Running heavy physics calculations (like geometry optimizations or molecular dynamics) is usually a messy process involving manual bash scripts, tangled dependencies, and inefficient use of hardware. 

Hessian Dynamics is my effort to clean this up. I am writing the software stack we wished we had, one that completely separates the core math of the physics engines from the messy infrastructure of job scheduling and hardware pinning.

### Repositories

* [**hess**](https://github.com/HessianDynamics/hess)
  The core physics driver. It acts as a unified wrapper around semi-empirical engines (like xTB) and machine learning force fields (like MACE). Instead of fighting with different input formats and parsing raw outputs, `hess` standardizes everything into clean trajectories and single-command executions.

* [**jobserver**](https://github.com/HessianDynamics/jobserver)
  A standalone, lightweight job queue. it is built to avoid freezing our terminals or fighting with heavy cluster schedulers just to run a few local parallel jobs. It automatically computes hardware limits, pins physical CPU cores, handles isolated sandboxes, and polls jobs in the background.

* **forge** *(Work in Progress)*
  My upcoming layer for running active learning loops, ML-driven molecular discovery, and automated conformer generation.

### Tech Stack
Most of my work is built in Python, heavily utilizing `ase` (Atomic Simulation Environment), PyTorch for neural network potentials, and strict POSIX process controls for the job scheduler.
