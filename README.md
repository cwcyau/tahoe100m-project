# tahoe100m-project

Project Lead: Christopher Yau

## Pre-requisite requirements: 

- Interest in cancer medicine
- Knowledge of Bayesian Statistics (Fundamentals of AI 1)
- Knowledge of Gaussian Process modelling (Fundamentals of AI 1)
- Knowledge of variational inference (Fundamentals of AI 1)

## Knowledge to be acquired:

- Hierarchical Bayesian Gaussian Process modelling
- Large-scale model implementations
- High-throughput cellular screening data analysis
- Bioinformatics

## Background
 
The Tahoe-100M data set is the largest single-cell perturbation data set in the world. The data contains 100 million single-cell gene expression profiles from 47 cancer lines, derived from 13 different organs, which have been subject to perturbation by 379 drugs targeting 325 genes. This dataset captures 17,813 unique cell line-drug conditions. 

## Problem

Let $$X_i \in \mathbb{R}^p$$ denote the $p$-dimensional gene expression profile for the $i$-th cell where $Y_i \in \\{1, \dots, T\\}$ denotes the corresponding cell type and $Z_i \in \\{1, \dots, D \\}$ the drug perturbation applied to the cell (includes no perturbation).
