# Heart Disease Classification with Polynomial Logistic Regression

## Overview

This repository contains code for classifying heart disease (AHD) using logistic regression with polynomial features. The analysis uses the `Heart.csv` dataset, which includes various health metrics to predict the presence of heart disease.

## Dataset

The dataset `Heart.csv` contains:

- **Chol**: Cholesterol level
- **MaxHR**: Maximum heart rate achieved
- **AHD**: Indicator for heart disease (1 for presence, 0 for absence)


## Model Training

1. **Logistic Regression**:
   - A logistic regression model is trained to predict AHD using `Chol` and `MaxHR` as predictors.
   - Polynomial features of degree 3 are used for both predictors.
   - The model is fit on the training data, and predictions are made.

2. **Accuracy Evaluation**:
   - The accuracy of the logistic regression model on the training set is calculated.



## Visualization

1. **Decision Boundary**:
   - The decision boundary is visualized using a mesh grid. The plot shows the decision boundary of the model, distinguishing between predicted classes.

## Counterfactual Analysis

1. **Sensitivity Analysis**:
   - The model's sensitivity to changes in the predictors (`Chol` and `MaxHR`) is analyzed.
   - The number of changes in predictions is measured by modifying each predictor by ±0.5 standard deviations.

## Results

- **Decision Boundary Visualization**:
  - The decision boundary plot distinguishes between predicted classes, showing how the model classifies the data.

- **Sensitivity Analysis**:
  - The model is more sensitive to changes in `MaxHR` compared to `Chol`.
