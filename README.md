# Trading At The Close

Local research workspace for the Kaggle competition **Optiver - Trading at the Close**.

This repository is centered on exploratory analysis in `eda.ipynb`, with a conda environment file and a local testing utility for time-series style inference loops.

## Project Structure

```text
.
|-- eda.ipynb
|-- environment.yml
|-- public_timeseries_testing_util.py
|-- data/
|   |-- train.csv
|   `-- test.csv
`-- example_test_files/
    |-- sample_submission.csv
    `-- revealed_targets.csv
```

## Environment Setup

This project uses conda and targets Python 3.11+.

```bash
conda env create -f environment.yml
conda activate trading-at-close
```

Core packages include:
- data and numerics: `pandas`, `numpy`, `polars`, `scipy`
- visualization: `matplotlib`, `seaborn`, `plotly`
- modeling: `scikit-learn`, `xgboost`, `lightgbm`, `catboost`, `pytorch`
- experimentation: `optuna`, `jupyter`

## Data

Expected local files:
- `data/train.csv`
- `data/test.csv`
- `example_test_files/sample_submission.csv`
- `example_test_files/revealed_targets.csv`

These folders are git-ignored, so data stays local.

## Current Status

- Main analysis lives in `eda.ipynb`
- Environment is defined in `environment.yml`
- Repository is set up for iterative local experimentation
