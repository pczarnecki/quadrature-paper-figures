# Sparse, Empirically Optimized Quadrature for Radiative Calculations
Code and data necessary to reproduce figures presented in our paper "Sparse, Empirically Optimized Quadrature for Radiative Calculations" (Czarnecki, Pincus, and Polvani, 2023). 

## Data
Line-by-line data necessary to perform the optimizations was used from the publicly-available <a href = 'https://confluence.ecmwf.int/display/CKDMIP/CKDMIP%3A+Correlated+K-Distribution+Model+Intercomparison+Project+Home'>CKDMIP</a> project (Hogan and Matricardi, 2020).

Optimization output files are found in the folder Results Files. The filenames are '[size S]\_linear\_annealing\_4angle\_100\_[cost function]\_[iteration index].h5'.

Each file contains: cost\_hist: the average cost function value in each block; temps: the annealing temperature in each block; W: the set of weights corresponding to the best model configuration; C: the best cost function value associated with this final configuration; blocks: the index of annealing blocks performed; half_level: the vertical index of model level; and S: the indeces of the best representative wavenumber set as determined by the optimization.

The folder ckdmipData contains results from ECCKD and RRTMGP models submitted to CKDMIP and plotted in the paper.

## Figures
All figures presented in the paper are found in the Paper Figures folder. The Jupyter Notebook 'Generate Figures.ipynb' creates these figures.
