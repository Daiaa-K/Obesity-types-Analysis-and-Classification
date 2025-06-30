# Obesity Types Analysis and Classification

This project analyzes lifestyle data to classify individuals into different obesity categories. It combines Python-based AutoML tools for modeling with an interactive Power BI dashboard to communicate insights visually.

## Project Overview

- **Objective:** Predict obesity types based on personal and lifestyle features.
- **Tools Used:** Python, FLAML, H2O, TPOT, Scikit-learn, Pandas, Power BI
- **Deliverables:** AutoML classification models and a Power BI dashboard

## Project Structure

- `Obesity analysis and classification.ipynb`: Main analysis and modeling notebook
- `FLaml.ipynb`, `h2o.ipynb`, `tpot.ipynb`: AutoML implementation notebooks
- `obesity_clean.csv`: Cleaned dataset used for training and testing
- `obesity type dashboard.pbix`: Power BI dashboard file
- `Obesity dashboard.png`: Dashboard screenshot
- `automl.log`, `logs.log`: Log files for model tracking

## Features

- Data cleaning, preprocessing, and exploratory analysis
- Model training using three different AutoML tools
- Classification of obesity levels based on health and behavior data
- Interactive Power BI dashboard to visualize trends and predictions

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Daiaa-K/Obesity-types-Analysis-and-Classification.git
   cd Obesity-types-Analysis-and-Classification
2. **(Optional) Set up a virtual environment and install dependencies:**

  ```bash
  python -m venv venv
  source venv/bin/activate  # or venv\Scripts\activate on Windows
  pip install -r requirements.txt
  ```
3. **Run the notebooks:**

    Obesity analysis and classification.ipynb for the full pipeline

    Other notebooks for AutoML-specific workflows

4. **Open the dashboard:**

    Use Power BI Desktop to open obesity type dashboard.pbix
