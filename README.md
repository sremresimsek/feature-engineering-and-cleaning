# 🧹 Data Cleaning & Missing-Value Studies

Hands-on Python notebooks exploring practical approaches to cleaning messy tabular data. These are **learning exercises**, not production preprocessing pipelines.

## Projects

### ☕ Cafe Sales — data cleaning
**Notebook:** [`missing_data_study/cafe_sales/cale_sales_cleaning.ipynb`](missing_data_study/cafe_sales/cale_sales_cleaning.ipynb)

**Files:** [dirty dataset](missing_data_study/cafe_sales/dirty_cafe_sales.csv) · [saved cleaned dataset](missing_data_study/cafe_sales/cleaned_cafe_sales.csv)

The notebook explores:
- Converting numeric-looking text with `pd.to_numeric(..., errors="coerce")`
- Treating `ERROR` and `UNKNOWN` as missing values
- Recovering some missing values using relationships between quantity, unit price, and total spent
- Removing remaining rows with missing values in selected numeric columns
- Filling selected categorical fields and dropping an unused date column

**Reproducibility note:** The included `cleaned_cafe_sales.csv` is a saved example output. The notebook's export step is currently **commented out**, so running it does not automatically overwrite that CSV.

### 🚢 Titanic — missing-value treatment
**Notebook:** [`missing_data_study/titanic/titanic_cleaning.ipynb`](missing_data_study/titanic/titanic_cleaning.ipynb) · [dataset](missing_data_study/titanic/titanic.csv)

Explores:
- Inspecting missing-value counts and distributions
- Comparing deletion approaches without permanently applying them to the dataset
- Comparing mean and median imputation for age
- Filling embarked values with the most common category
- Plotting the effects of different imputation strategies

**Note:** This notebook compares missing-data techniques rather than exporting a single finalized cleaned Titanic dataset.

## Tools

Python · pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook

## Running the notebooks

Open each notebook from its own directory to keep the relative CSV file paths working. Run cells in order in an environment with the listed packages installed.

## Scope

These projects demonstrate preprocessing practice and exploratory decisions. They do not include model training, formal data-quality tests, or deployment.
