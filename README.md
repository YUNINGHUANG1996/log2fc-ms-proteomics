# log2FC-ms-proteomics

This repository contains a Jupyter notebook for performing differential protein abundance analysis using mass spectrometry-based proteomics data. The pipeline computes log2 fold changes (log2FC) and statistical significance across customizable experimental groups.

## Features

- Reads and preprocesses proteomics data from Excel files.
- Cleans and reshapes data into a long format for modeling.
- Supports flexible group comparisons via linear modeling (`statsmodels`).
- Computes:
  - Log2 fold change (log2FC)
  - Raw p-values
  - FDR-adjusted p-values (Benjamini-Hochberg method)
- Outputs a tidy summary table of results for downstream visualization or interpretation.

## Usage

Update the input Excel file and define your experimental groupings and comparisons in the notebook. All group labels and comparison logic can be modified to match your study design.

## Requirements

- Python ≥ 3.8
- `pandas`
- `numpy`
- `statsmodels`
- `openpyxl`

Install dependencies via:

```bash
pip install pandas numpy statsmodels openpyxl
