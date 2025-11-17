# Obesity Types Analysis and Classification

This project analyzes lifestyle data to classify individuals into different obesity categories. It includes Python notebooks that run the analysis and AutoML experiments, and a Power BI dashboard for visualization.

## Project overview

* **Objective:** Predict obesity types from personal and lifestyle features.
* **Tools:** Python, Pandas, Scikit-learn, FLAML, H2O, TPOT, Matplotlib/Seaborn, Power BI
* **Outputs:** Cleaned dataset, notebooks with analysis and modeling, AutoML experiments, Power BI dashboard and exported PNG.

## Repository structure

```
dashboard/
  ├─ Obesity dashboard.png         # exported dashboard image
  └─ obesity type dashboard.pbix   # Power BI file

data/
  ├─ model data.csv
  ├─ obesity_clean.csv            # cleaned dataset used in notebooks
  └─ ObesityDataSet_raw_and_data_sinthetic.csv

notebooks/
  ├─ FLaml.ipynb                   # FLAML AutoML experiments
  ├─ h2o.ipynb                     # H2O AutoML experiments
  ├─ Obesity analysis and classification.ipynb   # main analysis and modeling notebook
  └─ tpot.ipynb                     # TPOT AutoML experiments

README.md
requirements.txt
```

## Notebooks — what I did (summary)

### `Obesity analysis and classification.ipynb` (main)

* Loaded the raw dataset and `obesity_clean.csv`.
* Inspected data types and basic quality checks (missing values, duplicates).
* Performed data cleaning and preprocessing:

  * Fixed datatypes and renamed columns where needed.
  * Handled missing values and obvious data-entry issues.
  * Basic feature encoding (categorical → numeric) and simple scaling where required.
  * Created a few derived features used in modeling.
* Exploratory Data Analysis (EDA):

  * Distribution plots, counts of obesity types, and relationships between age/weight/height.
  * Visual comparisons by gender, alcohol use, smoking, and transportation method.
* Modeling pipeline:

  * Train/test split and baseline models for comparison.
  * Ran AutoML experiments (see AutoML notebooks) and compared results.
  * Evaluated models with accuracy, precision/recall, F1-score, and confusion matrices.
  * Saved model artifacts and basic inference examples.
* Short notes in the notebook explain choices and where to find key outputs.

### AutoML notebooks (`FLaml.ipynb`, `h2o.ipynb`, `tpot.ipynb`)

* Each notebook runs an AutoML tool on the cleaned dataset and records the best models.
* Includes hyperparameter search, cross-validation, and a short evaluation summary.

## Dashboard — what’s included

* The Power BI dashboard (`obesity type dashboard.pbix`) visualizes key insights from the dataset.
* Main visuals in the exported PNG (`Obesity dashboard.png`):

  * Donut charts for Gender, Alcohol Drinking, Smoking, and Obesity Types.
  * Gauge widget showing average daily physical activity with related averages (age, height, weight).
  * Line chart: average weight by age and gender.
  * Grouped bar chart: obesity types by transportation mode and other comparison bars.
  * Top filters: Family History of Obesity, Gender, High Calorie Food, and Obesity Type.
* The dashboard is exported as a PNG for quick viewing.

## How to run

1. (Optional) Create and activate a virtual environment and install dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```
2. Open and run `notebooks/Obesity analysis and classification.ipynb` to reproduce the analysis and modeling steps.
3. AutoML experiments can be found in `notebooks/FLaml.ipynb`, `notebooks/h2o.ipynb`, and `notebooks/tpot.ipynb`.
4. Open `dashboard/obesity type dashboard.pbix` in Power BI Desktop or view the exported `dashboard/Obesity dashboard.png`.
