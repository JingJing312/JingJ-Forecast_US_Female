# Maximum Entropy Mortality Forecasting for U.S. Females (1933–2023)

**Author:** Jing Jing  
**Advisor:** Dr. Tatjana Miljkovic  

---

## Overview

This repository reproduces and extends the Maximum Entropy Mortality (MEM) framework for forecasting age-specific mortality, originally developed by Pascariu et al. (2019), to the U.S. female population. We leverage sex-specific annual life tables (ages 0–95) from the Human Mortality Database (HMD) covering 1933–2023.

Key features:

- **Moment-based density reconstruction**: Compute the first four statistical moments (mean, variance, skewness, kurtosis) of the annual age-at-death distribution and apply the MEM algorithm to recover full mortality density functions.
- **Rolling-window forecasting**: Out-of-sample evaluation across 18 sequential 20-year windows (e.g. fit 1960–1979 → forecast 1980–1999; …; fit 1984–2003 → forecast 2004–2023).
- **Benchmarking**: Six accuracy metrics (ME, MAE, MAPE, sMAPE, sMRAE, MASE) compared against a standard Lee–Carter implementation.
- **Reproducibility**: All data-processing, analysis scripts, and final figures are provided.  

---

## Repository Structure

