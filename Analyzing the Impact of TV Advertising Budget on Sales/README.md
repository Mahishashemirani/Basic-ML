# Advertising Budget vs Sales Analysis

This repository contains code that analyzes the relationship between advertising budgets (TV, Radio, Newspaper) and sales using a dataset from the file `Advertising.csv`. The analysis includes running linear regression, Ridge regression, and Lasso regression to compare how each model performs in predicting sales based on the budget allocated to each channel.

## Requirements

To run this code, you need the following Python libraries:

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

## data
- **TV**: Budget allocated to TV advertising
- **Radio**: Budget allocated to radio advertising
- **Newspaper**: Budget allocated to newspaper advertising
- **Sales**: The sales generated

  ## Code Overview

### 1. Data Loading

- The dataset is loaded into a pandas DataFrame.
- Basic information about the dataset is displayed using `df.info()`.


### 2. Scatter Plot

- A scatter plot is created to visualize the relationship between predictors and Sales.
- Axis labels and a title are added for clarity.



## Results

- The script generates scatter plots showing how TV advertising budgets relate to sales figures.
- The first plot shows the relationship for a subset of 7 rows, while the second plot visualizes all data points.
