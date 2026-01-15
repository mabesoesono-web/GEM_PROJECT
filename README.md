
## Mouse-GEM Flux Balance Analysis Project

This project presents a comprehensive constraint-based analysis of a genome-scale metabolic model (GEM) of Mus musculus using Flux Balance Analysis (FBA). The Mouse-GEM model is used to explore mammalian metabolic behaviour at a system level, focusing on metabolic network topology, flux distributions, environmental sensitivity, and gene essentiality.

The analyses were performed using COBRApy within a fully reproducible Conda-managed environment. The project is structured to support transparency, reproducibility, and extensibility for future metabolic simulations or comparative studies.

## Project objectives
The main goals of this project are to:

Characterise the topology and structural complexity of the Mouse-GEM metabolic network

Perform Flux Balance Analysis (FBA) using common objective functions:

Biomass production (growth)

ATP maintenance (energy demand)

Assess the impact of environmental inputs on model predictions:

Rich vs minimal media

Aerobic vs anaerobic conditions

Systematic nutrient uptake perturbations

Identify essential and non-essential genes through single-gene deletion simulations

Demonstrate the robustness and redundancy of mammalian metabolism captured by Mouse-GEM

## Repository structure
GEM_PROJECT/
│
├── data/               # Input data and model files (Mouse-GEM.xml)
├── notebook/           # Jupyter notebooks with all analyses
├── outputs/            # Generated figures and tables
├── environment.yml     # Conda environment specification
├── README.md           # Project overview (this file)

## Environment setup
All analyses were performed in a Conda-managed  environment to ensure reproducibility

conda env create -f environment.yml
conda activate gem_env

# Updating the environment
if dependencies are added or updated during development, export the updated configuration using:

conda env export > environment.yml

## Sofware installed
Python

COBRApy – constraint-based reconstruction and analysis

NumPy / Pandas – data handling

Matplotlib / Plotly – visualisation

Jupyter Notebook – interactive analysis and documentation

## Model selection and download

The genome-scale metabolic model used in this project is Mouse-GEM, obtained from the SysBioChalmers Metabolic Atlas repository.

Repository:
https://github.com/SysBioChalmers/Mouse-GEM/tree/main/model

Model file:
Mouse-GEM.xml

Format:
SBML (Systems Biology Markup Language)

## Model details

Organism: Mus musculus

Model name: Mouse-GEM

Version: v1.8.0

Source: Metabolic Atlas / SysBioChalmers

Format: SBML (.xml)

Scope: Genome-scale, generic mouse metabolism

Note: All analyses are documented and reproducible via the Jupyter notebooks provided in the notebook/ directory

## References
Key references related to Flux Balance Analysis, GEMs, and Mouse-GEM are provided in the accompanying report


