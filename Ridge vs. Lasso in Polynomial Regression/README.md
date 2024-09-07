# Ridge and Lasso Regression Analysis

## Overview

This script performs a Ridge and Lasso regression analysis on a dataset, exploring how different values of regularization parameters affect the coefficients of polynomial features.

## Requirements

To run this script, you need the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## Data

The script uses a dataset named `bacteria_train.csv`, which should be located in the same directory as the script. This dataset includes:

- **Spreading_factor**: Predictor variable.
- **Perc_population**: Response variable.

## Script Breakdown

1. **Library Imports**:
   - Imports required libraries and sets up `matplotlib` for better visuals.

2. **Data Loading**:
   - Reads the `bacteria_train.csv` file into a pandas DataFrame and displays the first few rows.

3. **Feature Preparation**:
   - Extracts the predictor and response variables.
   - Creates polynomial features up to a specified degree (7 in this case) and normalizes them.

4. **Ridge Regression Analysis**:
   - Defines a range of alpha values for Ridge regression.
   - Computes coefficients for each alpha value and plots how these coefficients vary with alpha.

5. **Lasso Regression Analysis**:
   - Defines a different range of alpha values for Lasso regression.
   - Computes coefficients for each alpha value and plots how these coefficients vary with alpha.

6. **Comparison Plot**:
   - Plots a comparison of Ridge and Lasso regression coefficients in a logarithmic scale to illustrate the differences between these regularization methods.

## Running the Script

To execute the script, save it as a `.py` file (e.g., `regression_analysis.py`) and run the following command in your terminal:

```bash
python regression_analysis.py
```

## Results

- The script generates visualizations showing how the coefficients of polynomial features change with different regularization parameters for both Ridge and Lasso regression.
- The final plot compares Ridge and Lasso regression in terms of their coefficient shrinkage effects.
