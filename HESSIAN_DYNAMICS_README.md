<div align="center">
  <h1>Hessian Dynamics</h1>
  <p><b>Simulating the fundamental laws of nature at scale.</b></p>
</div>

---

## 🔬 About Us

**Hessian Dynamics** is a computational physics and deep-tech AI laboratory. 

We merge foundational quantum mechanics with generative artificial intelligence to systematically explore molecular state spaces. Our infrastructure is built from the ground up for massive parallelization, bridging the gap between rigorous mathematical optimization (the Hessian) and modern neural network potentials.

We build the engines that forge new molecules.

---

## 🏗️ Core Infrastructure

Our open-source and internal repositories form a complete, vertically integrated scientific compute stack:

### ⚙️ [`hess`](https://github.com/HessianDynamics/hess)
**The Core Physics & Simulation Engine**
A unified orchestration layer that standardizes inputs, optimization lifecycles, and outputs across diverse computational backends (Semi-empirical xTB, Machine Learning Force Fields, DFT).

### 🖥️ [`jobserver`](https://github.com/HessianDynamics/jobserver)
**Autonomous Compute Orchestration**
A lightweight, standalone infrastructure layer that handles OS-level process management. It enforces strict physical core pinning (`OMP_PLACES=cores`), slot-based FIFO queueing, and silent background daemon polling to maximize L3 cache hits across compute clusters.

### 🧠 `forge` *(In Development)*
**Agentic Generative Intelligence**
The high-level AI layer that orchestrates the physics engines. `forge` handles active learning loops, automated conformer generation, and intelligent exploration of the Potential Energy Surface (PES).

---

## 🛠️ Technology Stack

* **Physics & Chemistry:** Semi-empirical methods (xTB), Density Functional Theory (DFT), `ase` (Atomic Simulation Environment).
* **Machine Learning Force Fields:** PyTorch, MACE (Equivariant Neural Network Potentials), NequIP.
* **Systems & HPC:** POSIX process control, OpenMP Hardware Affinity, Slurm/SSH remote execution.

---

<div align="center">
  <i>"Where mathematical absolute meets generative intelligence."</i>
</div>
