# Diabetes Risk Factor Analysis

## Project Purpose

This project was completed as part of the HSE 751 Programming for Health Data Science reproducibility exercise. The purpose of the analysis is to demonstrate a clear, reproducible analytical workflow using an example diabetes dataset.

The notebook documents the full workflow from environment setup and data validation through descriptive statistics, visualization, correlation analysis, inferential statistical testing, and interpretation of results. It is designed so that another data science team can reproduce the analysis from the provided dataset and notebook.

## Google Colab Notebook

The completed analysis can be viewed and executed in Google Colab:

[[Open the completed notebook in Google Colab]](https://colab.research.google.com/drive/1Ci2_J-RXajADlPmacMQLezed3NDX85vn?usp=sharing)

## Analysis Overview

The dataset contains 768 observations and nine variables. Eight patient characteristics are examined in relation to a binary diabetes outcome:

- `Pregnancies`
- `Glucose`
- `D_BP`
- `Skin_Thickness`
- `Insulin`
- `BMI`
- `Pedigree`
- `Age`
- `Outcome` — binary outcome coded as `0` for no diabetes and `1` for diabetes

The analytical workflow includes:

1. Data loading and structural validation
2. Descriptive statistics
3. Univariate and bivariate data visualization
4. Spearman correlation analysis
5. Independent-samples t-test comparing glucose by diabetes outcome
6. Univariable logistic regression evaluating the association between BMI and diabetes status
7. Reproducibility checks using a fixed random seed
8. Summary of findings and analytical limitations

The notebook also formally represents the dataset as a supervised binary classification problem, although a multivariable predictive machine-learning model is not trained or evaluated in this analysis.

## Dataset Source and Provenance

The analysis uses:

`Example Dataset_Diabetes.csv`

The CSV file is an example diabetes dataset provided for the HSE 751 reproducibility exercise. It contains 768 observations and nine variables.

The provided CSV serves as the source dataset for all analyses in the notebook. The original dataset is not modified by the notebook.

No external provenance beyond the course-provided dataset is assumed for this analysis.

## Required Software and Libraries

The analysis was developed for **Google Colab** using **Python 3**.

Required Python libraries are:

- `pandas` — data loading and manipulation
- `numpy` — numerical operations
- `matplotlib` — visualization
- `seaborn` — statistical visualization
- `scipy` — inferential statistical testing
- `statsmodels` — logistic regression and statistical inference

The notebook reports the Python and package versions used during execution in the **Setup and Environment** section. These reported versions should be consulted when reproducing the computational environment exactly.

## Installation and Setup

Google Colab includes the required libraries in its standard Python environment. If the packages are not already available, they can be installed with:

```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels
