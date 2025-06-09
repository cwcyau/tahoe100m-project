# tahoe100m-project

**Project Lead:** Christopher Yau

## Pre-requisite requirements: 

- Interest in cancer medicine
- Knowledge of Bayesian Statistics (Fundamentals of AI 1)
- Knowledge of Gaussian Process modelling (Fundamentals of AI 1)
- Knowledge of variational inference (Fundamentals of AI 1)
- Python (Software Engineering)

## Knowledge to be acquired:

- Hierarchical Bayesian Gaussian Process modelling
- Large-scale model implementations in PyTorch
- High-throughput cellular screening data analysis
- Bioinformatics

## Background
 
The [Tahoe-100M](https://www.biorxiv.org/content/10.1101/2025.02.20.639398v1.full) data set is the largest single-cell perturbation data set in the world. The data contains 100 million single-cell gene expression profiles from 47 cancer lines, derived from 13 different organs, which have been subject to perturbation by 379 drugs targeting 325 genes. This dataset captures 17,813 unique cell line-drug conditions.

## Problem

Let $X_i \in \mathbb{R}^p$ denote the $p$-dimensional gene expression profile for the $i$-th cell in the training data where $Y_i \in \\{1, \dots, T\\}$ denotes the corresponding cell type and $Z_i \in \\{0, \dots, D \\}$ the drug perturbation applied to the cell (includes no perturbation labelled 0). 

We want to construct a model for $p(X^d | X^0, Z^0 = 0, Y^d = t, Z^d = k )$ to predict the gene expression $X^d$ for a cell of type $t$ for drug $k$ with unperturbed expression $X^0$.

In [Xing and Yau (2025)](https://www.biorxiv.org/content/10.1101/2025.03.26.645455v1), we have used Gaussian Process models to provide an explainable and scalable hierarchical Bayesian modelling approach to address this problem.
