# CART_immuno_metabolic_pipeline

Immuno-metabolic profiling pipeline for CAR T cells — Moraly et al., *Nature Immunology* manuscript, 2026.

<p align="center">
  <img width="600" alt="Overview of the immuno-metabolic profiling pipeline" src="https://github.com/user-attachments/assets/b6c7894e-5b72-46a3-9ee2-13400e23a681" />
</p>

## Overview

This repository contains the processed data and analysis code used to generate **Figure 1** and **Extended Data Figure 1** of the manuscript by Moraly et al.

These figures describe the development and validation of an integrated immuno-metabolic profiling pipeline for CAR T cells. The approach combines multiplex cytokine measurements with high-dimensional spectral cytometry to characterize protein synthesis, mitochondrial activity, metabolite-transporter expression, and metabolic pathway dependencies at single-cell resolution.

## Repository contents

- [`data/`](data/): processed data used to generate Figure 1 and Extended Data Figure 1
- [`code/`](code/): data-analysis and figure-generation scripts

```text
CART_immuno_metabolic_pipeline/
├── README.md
├── data/
│   ├── cytokines.csv
│   ├── metabolic_features_protein_synthesis.csv
│   └── single_cell.csv
└── code/
    ├── cytokine_dynamics.ipynb
    └── integrative_analysis.ipynb
```

## Data availability

The processed data required to reproduce Figure 1 and Extended Data Figure 1 are provided in the [`data/`](data/) directory.
