# Polynomial Regression Analysis

## Overview

This script performs polynomial regression on a dataset to determine the optimal polynomial degree based on training and validation errors. It uses Mean Squared Error (MSE) to evaluate the performance of models with different polynomial degrees and visualizes the results.

## Requirements

To run this script, ensure you have the following Python libraries installed:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install numpy pandas matplotlib scikit-learn
```

## Data

The script uses a dataset named `dataset.csv`. Ensure this file is located in the same directory as the script. The dataset should contain:

- **x**: Predictor variable.
- **y**: Response variable.


## Script Breakdown

### 1. Library Imports

- Imports necessary libraries including data manipulation, visualization, and machine learning modules.

### 2. Data Loading

- Reads the dataset `dataset.csv` into a pandas DataFrame.
- Extracts predictor (`x`) and response (`y`) variables from the DataFrame.

### 3. Train-Validation Split

- Splits the dataset into training (75%) and validation (25%) sets using a fixed random seed (`random_state=1`).

### 4. Polynomial Feature Transformation and Model Training

- Iterates through polynomial degrees from 1 to 18.
- Computes polynomial features for both training and validation sets.
- Trains a Linear Regression model for each degree without adding an extra intercept (as `PolynomialFeatures` adds one).
- Evaluates the model using Mean Squared Error (MSE) on both training and validation sets.

### 5. Optimal Polynomial Degree

- Identifies the polynomial degree with the lowest validation MSE.

### 6. Visualization

- Plots MSE vs. polynomial degree for both training and validation sets.
- The plot uses a logarithmic scale for the y-axis to better visualize the errors.



## Running the Script

To execute the script, save it as a `.py` file (e.g., `polynomial_regression_analysis.py`) and run the following command in your terminal:

```bash
python polynomial_regression_analysis.py
```

## Output

- The script prints the optimal polynomial degree based on the validation MSE.
- It generates a plot showing the training and validation MSEs as a function of polynomial degree.
