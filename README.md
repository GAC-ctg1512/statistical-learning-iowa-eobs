# MHYWI05 — Statistical Learning for Earth System Sciences

Project report and analysis code for the module MHYWI05 at TU Dresden (Summer Semester 2026).

## Author

Galib Ahmed Chowdhury
M.Sc. Hydro Science and Engineering (TU Dresden)

## Overview

Two analyses are presented:

1. **Iowa crop yield prediction** — comparing best-subset and lasso regression
   under random versus year-parity train/test splits, illustrating the effect
   of spatial dependence on cross-validation.

2. **European climate trend analysis** — per-grid-cell linear trends in
   temperature and precipitation (1950–2025), with Benjamini–Hochberg FDR
   correction for multiple testing.

## Repository structure
.
├── report/ LaTeX source for the report
│ ├── main.tex
│ ├── title.tex
│ └── TUDlogo.png
├── code/ R analysis script
│ └── analysis.R
├── figures/ Generated figures (PNG)
├── report.pdf Compiled report
└── README.md


## Reproducing the analysis

1. Obtain the three data files from the course materials
   (`Iowa.RData`, `temperature.nc`, `precipitation.nc`)
2. Place them in a working directory
3. Open `code/analysis.R` in R or RStudio
4. Update the `setwd()` path at the top of the script
5. Run the script end-to-end

The script regenerates all five figures and prints the numerical results
reported in the paper.

## Requirements

- R (>= 4.2.0)
- R packages: `ncdf4`, `leaps`, `glmnet`, `fields`, `rworldmap`
- LaTeX with `pdflatex` (for compiling the report)

## License

Course submission; not licensed for redistribution.

