# DisperPy: Python-based Dispersion Calculator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**DisperPy** is a Python implementation of the Semi-Analytical Finite Element (SAFE) method for computing guided wave dispersion curves in waveguides of arbitrary cross-section. This repository supports the research presented in the paper:

> **"Rigorous foundations of adaptive mode tracking in single-parametric Hermitian eigenvalue problems: existence theorems, error indicators, and application to SAFE dispersion analysis"**  
> by Dong Xiao, Zahra Sharif-Khodaei, and M. H. Aliabadi.

The code implements the **adaptive wavenumber sampling algorithm** proposed in the paper, which robustly tracks modes through veering (avoided crossing) regions and handles symmetry-protected degeneracies.

## ✨ Features

- **SAFE Formulation**: For waveguides with arbitrary cross-sections and material anisotropy.
- **Adaptive Mode Tracking**: Automatically refines the wavenumber grid based on a rigorous error indicator to ensure correct mode identification.
- **Subspace Tracking**: Handles symmetry-protected degenerate modes (e.g., in pipes) using a rotation-invariant Subspace MAC.
- **Reproducibility**: All numerical examples from the paper are fully reproducible.

## 🚀 Getting Started

### Prerequisites

The code requires Python 3.8+ with the following packages:
- `numpy`, `scipy`, `matplotlib`
- `meshio` (for mesh handling)
- `h5py` (for reading result files)

### Installation

Clone the repository:
```bash
git clone https://github.com/dongxiao96/DisperPy.git
cd DisperPy
