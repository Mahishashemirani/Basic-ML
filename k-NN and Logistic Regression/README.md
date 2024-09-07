# Heart Disease Prediction Analysis

## Overview
This repository contains code to analyze and predict the presence of heart disease using two different models: k-Nearest Neighbors (k-NN) and Logistic Regression. The analysis is based on the `Heart.csv` dataset, which includes various features related to heart health.


## Dataset
The dataset `Heart.csv` includes patient data with the following key columns:
- **Age**: Age of the patient
- **AHD**: Presence of heart disease (Yes/No)
  
## Data Preparation
- The response variable `AHD` is transformed into a binary indicator (1 for "Yes", 0 for "No").
- The data is split into training (75%) and validation (25%) sets.


## Models

### k-Nearest Neighbors (k-NN)
- **Model**: `KNeighborsClassifier`
- **Parameter**: `k=20`
- **Training**: Fit the k-NN model on the training set using age as the predictor.
- **Predictions**: Generate both classification and probability predictions for the training data.

### Logistic Regression
- **Model**: `LogisticRegression`
- **Parameter**: No regularization (`penalty=None`)
- **Training**: Fit the logistic regression model on the training set using age as the predictor.
- **Coefficients**: Extract and interpret the coefficients to determine the odds of having heart disease.


## Results

### Predictions and Probabilities

- **k-NN**:
  - Pure classifications and probability estimates for the training data.

- **Logistic Regression**:
  - Coefficient estimates for the logistic regression model.
  - Estimated probability of having heart disease for a 60-year-old.

### Accuracy

- Compute and compare the accuracy of both models on both training and validation sets.

### Visualization

- **Plots**:
  - Plot the observed data along with model predictions for k-NN and logistic regression.
  - Visualize different types of predictions (classifications and probabilities).

