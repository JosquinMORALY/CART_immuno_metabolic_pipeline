# CART_immuno_metabolic_pipeline

Immuno-metabolic profiling pipeline for CAR T cells — Moraly et al., *Nature Immunology* manuscript, 2026.

<p align="center">
  <img width="600" alt="Overview of the immuno-metabolic profiling pipeline" src="https://github.com/user-attachments/assets/b6c7894e-5b72-46a3-9ee2-13400e23a681" />
</p>

## Overview

This repository contains the processed data and analysis code used to generate **Figure 1** and **Extended Data Figure 1**.

The immuno-metabolic profiling pipeline combines longitudinal measurement of 12 cytokines and chemokines over 72 hours with extracellular flux analysis and high-dimensional spectral flow cytometry. Metabolic profiling includes glycolysis, oxidative phosphorylation, spare respiratory capacity, protein synthesis, mitochondrial dependence, mitochondrial mass, membrane potential, ROS, and GLUT1 and ASCT2 expression.

## Repository contents

* [`data/`](data/) — processed, analysis-ready datasets from 4 donors and 6 CAR constructs.

* [`code/`](code/):

  * **`01_cytokine_analysis.ipynb`** — analysis of global cytokine secretion (integrated log-transformed cytokine concentrations) and high-dimensional cytokine dynamics, including low-dimensional projection and extraction of kinetic parameters, adapted from Achar et al., *Science* (2022), DOI: 10.1126/science.abl5311.
  * **`02_metabolic_parameters_and_score.ipynb`** — analysis and integration of metabolic features, including calculation of a PCA-based composite metabolic score summarizing extracellular flux, nutrient-transporter expression, and mitochondrial parameters.

## Repository contents

- [`data/`](data/) — processed, analysis-ready datasets:
  - `cytokineConcentrationPickleFile-20221003-MetMYCAR_1.pkl` — longitudinal cytokine and chemokine measurements used for cytokine dynamics analyses.
  - `metabo_all_act1.xlsx` — metabolic profiling dataset containing extracellular flux and spectral flow cytometry-derived parameters.

- [`code/`](code/):
  - `01_cytokine_analysis.ipynb` — analysis of global cytokine secretion (integrated log-transformed cytokine concentrations) and high-dimensional cytokine dynamics, including low-dimensional projection and extraction of kinetic parameters, adapted from Achar et al., *Science* (2022), DOI: 10.1126/science.abl5311.
  - `02_metabolic_parameters_and_score.ipynb` — analysis and integration of metabolic features, including calculation of a PCA-based composite metabolic score.

## Data availability

Processed data required to reproduce the corresponding analyses are provided in the [`data/`](data/) directory.
