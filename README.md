# Data Cleaning & Missing-Value Studies

Course-based learning notebooks for exploring messy tabular data. These are educational exercises, not independent production pipelines.

## Cafe Sales

[Notebook](missing_data_study/cafe_sales/cafe_sales_cleaning.ipynb) · [Raw data](missing_data_study/cafe_sales/dirty_cafe_sales.csv)

Convert numeric fields, recover missing values using quantity, price and total relationships, infer item names only from unique prices, and preserve unknown categories. Report nonpositive quantities/prices and inconsistent totals before exporting the cleaned CSV locally. The fixed price mapping is an assumption of this exercise, not a general retail rule. The date column is dropped as in the original exercise.

## Titanic

[Notebook](missing_data_study/titanic/titanic_cleaning.ipynb) · [Data](missing_data_study/titanic/titanic.csv)

Compare row/column deletion, mean and median age imputation, and categorical mode imputation. This notebook is a comparison of methods rather than a finalized cleaned dataset.

## Run locally

Create a virtual environment, install `python -m pip install -r requirements.txt`, and open `python -m jupyter notebook`. Run each notebook from its own folder. See [DATA_SOURCES.md](DATA_SOURCES.md) for provenance limitations. The edited Cafe Sales notebook has cleared outputs and must be rerun to regenerate its cleaned CSV. Dependencies and runtime behavior have not yet been verified.
