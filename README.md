# helical-ct-reconstruction
Supporting code for an MSc dissertation on iterative helical CT reconstruction, regularisation, and geometric model mismatch.


# Iterative Cone-Beam CT Reconstruction

Supporting code for my MSc Applied Mathematics dissertation at the University of Manchester.

This repository contains the computational experiments used to investigate iterative reconstruction in helical cone-beam CT. The experiments focus on acquisition sampling, measurement noise, regularisation, geometric model mismatch, data redundancy, and data-driven stopping.

## Contents

The main notebook, `Iterative_Cone-Beam_CT--Coding.ipynb`, contains the complete computational workflow used for the dissertation.

The experiments include:

- construction of a numerical phantom and helical cone-beam CT acquisition geometry;
- simulation of projection data using CIL and the ASTRA Toolbox;
- iterative reconstruction and diagnostic utilities;
- acquisition-sampling experiments, including helical pitch and projection density;
- investigation of measurement noise and LSQR semi-convergence;
- Tikhonov regularisation and discrepancy-principle parameter selection;
- Tam--Danielsson (TD) window construction and reconstruction;
- geometric model-mismatch experiments involving source-to-detector distance (SDD), centre-of-rotation (COR), and axis displacement;
- continuous weighting of redundant measurements outside the TD window;
- data-driven prediction of LSQR stopping iterations using early-iteration features and random-forest regression.

The notebook also contains the code used to generate the principal numerical results and figures presented in the dissertation.

## Software

The experiments were implemented in Python using the Core Imaging Library (CIL) and the ASTRA Toolbox for GPU-accelerated projection and backprojection. The main Python packages used include:

- NumPy
- Matplotlib
- pandas
- SciPy
- scikit-learn
- Core Imaging Library (CIL)
- ASTRA Toolbox

The computational experiments were run using Python 3.12, CIL 26.0.0, and ASTRA Toolbox 2.5.0.

## Running the notebook

The notebook is organised sequentially, beginning with the common reconstruction setup and followed by the individual numerical experiments.

Some experiment blocks are computationally expensive and can be disabled when previously computed results are available. GPU acceleration is required for the ASTRA projection and backprojection operations used in the reconstruction experiments.

## Dissertation

This repository accompanies the MSc dissertation:

**"[FINAL DISSERTATION TITLE]"**

MSc Applied Mathematics  
Department of Mathematics  
The University of Manchester  
2026

## Author

Jiayu Di
