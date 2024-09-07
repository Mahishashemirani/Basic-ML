# TV Advertising Budget vs Sales Analysis

This repository contains code that analyzes the relationship between TV advertising budgets and sales using a dataset from the file `Advertising.csv`. The dataset is read using the `pandas` library, and the relationship is visualized with a scatter plot using `matplotlib`.

## Requirements

To run this code, you need the following Python libraries:

- `pandas`
- `matplotlib`

You can install these libraries using pip:

```bash
pip install pandas matplotlib
```

## data
- **tv**: Budget allocated to TV advertising
- sales: The sales generated

  ## Code Overview

### 1. Data Loading

- The dataset is loaded into a pandas DataFrame.
- Basic information about the dataset is displayed using `df.info()`.

### 2. Data Preview

- A new DataFrame `df_new` is created by selecting the first 7 rows of the dataset.
- The contents of this new DataFrame are printed to verify the selection.

### 3. Scatter Plot

- A scatter plot is created to visualize the relationship between TV and Sales.
- Axis labels and a title are added for clarity.

### 4. Full Dataset Plotting

- An additional plot is generated to visualize all data points.


## Running the Script

To run the script, execute the following command in your terminal:

```bash
python tv_advertising_analysis.py
```

## Results

- The script generates scatter plots showing how TV advertising budgets relate to sales figures.
- The first plot shows the relationship for a subset of 7 rows, while the second plot visualizes all data points.
