# Undergraduate Statistics Project

**Statistical analysis and predictive modeling of biomedical datasets using R.**

## Overview

This undergraduate project explores statistical methods for understanding biomedical data, investigating relationships between clinical variables, and evaluating predictive models. The work is documented in a Jupyter notebook containing R code, visualizations, and methodological explanations.

The notebook begins with an exploratory analysis of a cardiovascular dataset and then focuses on the **Pima Indians Diabetes** dataset from the `mlbench` R package.

## Objectives

- Explore clinical variables using descriptive statistics and visualizations.
- Investigate correlations and statistical distributions.
- Develop and compare multiple linear regression models.
- Build logistic regression models for diabetes classification.
- Evaluate predictive performance and model assumptions.
- Compare multinomial logistic regression with k-nearest neighbors (KNN).

## Datasets

### Cardiovascular dataset

The initial investigation uses a `cardio_train.csv` file, including cardiovascular measurements and risk factors. The notebook documents data cleaning, BMI calculation, correlation analysis, k-means clustering, and exploratory regression models. **This CSV file is not included in the supplied notebook** and must be provided separately to reproduce that section.

### Pima Indians Diabetes

The main analysis uses `PimaIndiansDiabetes` and `PimaIndiansDiabetes2`, available through the R package `mlbench`. The variables include pregnancies, glucose, blood pressure, triceps skinfold thickness, insulin, body mass index, diabetes pedigree function, age, and diabetes status.

The notebook also explores mean imputation for missing values in `PimaIndiansDiabetes2` when assessing regression predictions.

## Methods

| Area | Techniques |
| --- | --- |
| Descriptive statistics | Mean, median, mode, variance, standard deviation, quantiles, skewness, kurtosis |
| Visualization | Histograms, boxplots, bar charts, scatterplot matrices |
| Statistical exploration | Correlation matrices, Shapiro–Wilk tests |
| Regression | Multiple linear regression, model selection, residual diagnostics |
| Classification | Binary and multinomial logistic regression, KNN |
| Clustering | K-means and elbow method (initial cardiovascular analysis) |
| Evaluation | R², AIC, BIC, residual errors, confusion matrices, accuracy and classification diagnostics |

## Repository contents

```text
Undergraduate-Statistics-Project/
├── README.md
└── STATISTICS_DELIVERABLE_2_.ipynb
```

## Getting started

1. Install **R** and a notebook environment that supports an **R kernel** (such as Jupyter with IRkernel).
2. Open `STATISTICS_DELIVERABLE_2_.ipynb` with the R kernel.
3. Run the package installation and loading cells. The notebook lists packages including `tidyverse`, `ggplot2`-related tools, `psych`, `GGally`, `caret`, `mlbench`, `nnet`, `pROC`, and `ResourceSelection`.
4. To run the initial cardiovascular analysis, place `cardio_train.csv` in the notebook's working directory.
5. Run the cells in order. The Pima Indians Diabetes analysis loads its data directly from `mlbench`.

**Note:** The notebook contains exploratory code and model comparisons. Some sections may require adjustments to package versions, variable types, or preprocessing to run independently. Its reported model comparisons should be treated as educational analyses rather than clinically validated predictive systems.

## Project structure

1. **Initial cardiovascular exploration:** data cleaning, clustering, linear regression, and logistic regression.
2. **Descriptive analysis:** distributions and summary statistics for diabetes-related variables.
3. **Correlation analysis:** relationships between biomedical measurements.
4. **Linear regression:** model fitting, comparison, and diagnostic plots.
5. **Prediction analysis:** evaluation using the alternative diabetes dataset and missing-value imputation.
6. **Classification:** binary logistic regression for diabetes status.
7. **Model comparison:** multinomial logistic regression versus KNN for predicting pregnancy counts.

## Technologies

**Language:** R  
**Environment:** Jupyter Notebook with R kernel  
**Main libraries:** `tidyverse`, `psych`, `GGally`, `caret`, `mlbench`, `nnet`, `pROC`, `lmtest`, `performance`

## Disclaimer

This repository is an educational statistics project. Its analyses and models are not intended for clinical diagnosis or medical decision-making.
