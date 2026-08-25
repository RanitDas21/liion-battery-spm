# ME698V Mid-Term Project — Single-Particle Model (SPM) of a Li-ion Cell

**Course:** ME698V — Physics-Based Modeling of Li-ion Batteries
**Cell chemistry:** Carbon | LiPF₆ Electrolyte | NMC111

## Overview

This project develops a Single-Particle Model (SPM) for a Carbon | LiPF₆ | NMC111 lithium-ion cell in three stages:

1. **Carbon anode half-cell** — modeled using Verbrugge and Koch's thermodynamic interaction formalism.
2. **NMC111 cathode half-cell** — modeled with an analogous formalism, with interaction parameters fit to reported voltage–capacity data.
3. **Full-cell response** — the two half-cell models are combined, first at equilibrium and then including Butler–Volmer kinetics at the particle surface.

## Repository Structure

```
├── Report/
│   ├── ME698V_MidTerm_Report.tex   # LaTeX source of the project report
│   └── ME698V_MidTerm_Report.pdf   # Compiled report
├── Codes/
│   ├── Problem1.ipynb              # Carbon anode half-cell model
│   ├── Problem2.ipynb              # NMC111 cathode half-cell model
│   ├── Problem3.ipynb              # Cathode parameter fitting
│   ├── Problem4.ipynb              # Full-cell equilibrium + Butler-Volmer kinetics
│   └── cathode_fit_params.npy      # Fitted NMC111 interaction parameters
└── Output/
    ├── Problem1.png
    ├── Problem2.png
    ├── Problem3.png
    └── Problem4.png
```

## Usage

Each notebook in `Codes/` corresponds to one problem in the report and can be run independently in Jupyter. `Problem2.ipynb`/`Problem3.ipynb` save/consume `cathode_fit_params.npy` for the fitted cathode parameters used downstream.

See `Report/ME698V_MidTerm_Report.pdf` for the full derivations, methodology, and results.

## Author

Ranit Das

M.Tech - Solid Mechanics and Design

IIT Kanpur
