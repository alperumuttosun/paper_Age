# Cohort-adjusted Myers index

R code to estimate a cohort-adjusted Myers index from repeated single-year age distributions, applied to Eurostat population data for European countries and NUTS regions.

## Data

Eurostat dataset `demo_r_d2jan` (population on 1 January by age, sex and NUTS 2 region). The script downloads it automatically and saves a local copy, so the download happens only once.

## Requirements

R (≥ 4.1), R version used: xxx. Packages: `splines`, `MASS` and `eurostat` (installed automatically if missing).

## How to run

Set `base_A` (or `base_B`) in section 0 of the R script to your working folder and run the script. Results are written to the subfolder `paper_age`. Finished blocks are skipped, so an interrupted run resumes where it stopped. A full run takes several hours because of the simulations.

## Steps

| Step | Content |
|---|---|
| 01 | Data download and preparation |
| 02 | Identifiability by observation design; classical Myers index |
| 03 | First index on ages 23–72; Figure 1 |
| 05 | Poisson estimator, alternative age ranges, stability over time |
| 06 | Final index, score test and intervals for all units; main simulation |
| 07 | Sensitivity analyses; digit effects; figures |
| 08 | Additional checks and simulations |
| 09 | Decomposition of the classical–adjusted difference; weak identification |

Step 04 of the development version is not needed. Figures are saved as PDF and 1600 dpi PNG.
