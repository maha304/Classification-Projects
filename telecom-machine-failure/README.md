# Telecom Machine Failure Analysis

## Problem

Unexpected telecom machine failures can interrupt service and increase maintenance costs. The available operational logs are inconsistent and require substantial preparation before they can support predictive maintenance.

## Questions Answered

- What patterns distinguish failure days from normal operating days?
- Which measurements and engineered features are associated with failure?
- Which variables are redundant or strongly correlated?
- Can the raw logs be transformed into a reliable modeling dataset?

## Work Completed

- Cleaned and standardized more than 700 days of machine logs from 2015–2017.
- Corrected date alignment, missing values, duplicates, and inconsistent columns.
- Engineered 100+ temporal, operational, and statistical features.
- Completed exploratory analysis of class patterns, distributions, outliers, and correlations.
- Produced analysis-ready datasets for the modeling phase.

![Machine failure correlation matrix](../assets/machine-failure-correlation.png)

## Current Status

**Data preparation and EDA are complete. Predictive model development is the next phase.** No production model performance is claimed yet.

## Repository Contents

- `data/` — processed datasets and labels
- `notebooks/01-data-preparation.ipynb` — cleaning and feature engineering
- `notebooks/02-exploratory-analysis.ipynb` — exploratory data analysis

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Open the preparation notebook first, followed by the EDA notebook.

## Tools

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, and Jupyter Notebook.

