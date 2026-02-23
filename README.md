# ACh in CA1: light/dark open-field photometry

This repository contains analysis code and raw exported data for a fiber photometry study measuring hippocampal CA1 acetylcholine (ACh; GRAB-ACh) during free exploration in an open field under two illumination conditions (Light vs Dark). The code reproduces the main analyses and figures reported in the manuscript.

## Repository contents

- `code/`  
  Analysis scripts / notebooks (R/Rmd) to preprocess exported data tables, generate figures, and run statistical models.

- `data-raw/`  
  Raw fluorescence data and DeepLabCut tracking data used as inputs to the analysis pipeline (e.g., binned photometry and behavioral variables).  
  **Note:** This repository does not include original video files or DeepLabCut model itself.

## What this repo enables

Using the files in `data-raw/` and the scripts in `code/`, a user can:
- reproduce the key preprocessing steps (binning / filtering / optional immobility subset),
- regenerate figures (e.g., fluorescence vs speed; log-speed models; model diagnostics),
- rerun the primary statistical models (e.g., mixed-effects models with lightness, speed/log(speed), and interactions),

## Reproducing the analyses

1. Install R (>= 4.2) and RStudio.
2. Open the main analysis file in `code/` (e.g., `GRAB_ACh-OF-LIGHTS (Short).Rmd`).
3. Install required packages (see the first code chunk / `renv.lock` if provided).
4. Run the script/notebook to regenerate results.
