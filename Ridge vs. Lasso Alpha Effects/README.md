# Ridge and Lasso Regression Analysis

## Overview

This script performs Ridge and Lasso regression on a dataset to compare the effect of regularization on polynomial regression coefficients. It visualizes how different alpha values affect the coefficients of polynomial features for Ridge and Lasso regularizations.

## Requirements

Ensure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## Data

The script uses a dataset named `bacteria_train.csv`.
- `Spreading_factor`: Predictor variable.
- `Perc_population`: Response variable.

  ## Script Breakdown

1. **Library Imports**:
   - Imports necessary libraries including data manipulation, visualization, and machine learning modules.

2. **Data Loading**:
   - Reads the dataset `bacteria_train.csv` into a pandas DataFrame.
   - Extracts predictor (`x`) and response (`y`) variables from the DataFrame.

3. **Polynomial Feature Transformation**:
   - Transforms the predictor variable into polynomial features up to a maximum degree (`maxdeg = 7`).
   - Normalizes the polynomial features to have mean 0 and variance 1.

4. **Ridge Regression Analysis**:
   - Iterates over a range of alpha values (from 10 to 120).
   - Computes Ridge regression coefficients for each alpha value.
   - Plots the variation of Ridge coefficients as a function of alpha values.

5. **Lasso Regression Analysis**:
   - Iterates over a range of alpha values (from 1e-4 to 1e-1).
   - Computes Lasso regression coefficients for each alpha value.
   - Plots the variation of Lasso coefficients as a function of alpha values.

6. **Comparison of Ridge and Lasso**:
   - Compares Ridge and Lasso regression by plotting the coefficients for both methods on the same plot.
   - Uses a logarithmic scale to highlight differences in how Ridge and Lasso shrink coefficients.

## Running the Script

To execute the script, save it as a `.py` file (e.g., `regression_analysis.py`) and run the following command in terminal:

```bash
python regression_analysis.py
```

## Output

- **Ridge Regression Plot**: Shows the variation of Ridge coefficients for different polynomial degrees as a function of alpha values.
- **Lasso Regression Plot**: Shows the variation of Lasso coefficients for different polynomial degrees as a function of alpha values.
- **Comparison Plot**: Highlights the differences between Ridge and Lasso regression by plotting the coefficients on a logarithmic scale.


