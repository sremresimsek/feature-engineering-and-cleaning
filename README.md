# Feature Engineering & Data Cleaning

**Guided data cleaning coursework & practical notebooks** · Python · pandas · NumPy

This repository collects the data cleaning exercises I practiced while learning to handle missing values, inconsistent records and categorical data.

**Scope and ownership:** These are guided learning exercises, not independently designed production pipelines.

## Study notebooks

### Cafe Sales

[Notebook](missing_data_study/cafe_sales/cafe_sales_cleaning.ipynb) · [Raw data](missing_data_study/cafe_sales/dirty_cafe_sales.csv)

Recover missing numeric values using quantity, unit price and total relationships. Infer item names only when prices uniquely identify them, preserve unknown categories, and check nonpositive values and inconsistent totals before exporting the cleaned CSV. The fixed price mapping is specific to this exercise.

### Titanic

[Notebook](missing_data_study/titanic/titanic_cleaning.ipynb) · [Data](missing_data_study/titanic/titanic.csv)

Compare row and column deletion, mean and median age imputation, and categorical mode imputation. This is a comparison of cleaning methods rather than a finalized cleaned dataset.

## Getting started

1. Create and activate a Python virtual environment.
2. Install dependencies: `python -m pip install -r requirements.txt`.
3. Open Jupyter: `python -m jupyter notebook`.
4. Run each notebook from its own directory. The Cafe Sales notebook generates `cleaned_cafe_sales.csv` locally.

## Data and reproducibility

The notebooks were run locally during the cleanup using Python 3.12. Dependency versions are not locked. See [DATA_SOURCES.md](DATA_SOURCES.md) for dataset information and provenance limitations.
