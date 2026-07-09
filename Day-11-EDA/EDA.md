# Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) is the process of understanding and exploring a dataset before building a machine learning model. It helps you identify patterns, outliers, missing values, and relationships between variables.

## 1. Univariate Analysis

Analyzes one variable at a time.

### Purpose

- Understand the distribution
- Find missing values
- Detect outliers
- Calculate summary statistics

### Examples

- Mean, median, mode
- Standard deviation
- Histogram
- Box plot
- Bar chart for categorical data

### Example

Analyze only the Age column.

## 2. Bivariate Analysis

Analyzes the relationship between two variables.

### Purpose

- Find correlations or associations
- Compare groups
- Understand how one variable affects another

### Examples

- Scatter plot for numerical vs numerical
- Correlation matrix
- Box plot for categorical vs numerical
- Grouped bar chart for categorical vs categorical

### Example

Relationship between Age and Salary.

## 3. Multivariate Analysis

Analyzes three or more variables together.

### Purpose

- Discover complex relationships
- Identify feature interactions
- Reduce dimensionality

### Examples

- Pair plot
- Heatmap
- 3D scatter plot
- Principal Component Analysis (PCA)
- Parallel coordinates plot

### Example

Study how Age, Salary, and Experience together affect Job Level.

## Types of Variable Combinations

| Analysis Type | Variables | Example                              |
| ------------- | --------- | ------------------------------------ |
| Univariate    | 1         | Age                                  |
| Bivariate     | 2         | Age vs Salary                        |
| Multivariate  | 3+        | Age, Salary, Experience -> Job Level |

## Common EDA Workflow

1. Load the dataset.
2. Check dataset shape (rows x columns).
3. Inspect data types.
4. Check missing values.
5. Remove duplicates.
6. Perform univariate analysis.
7. Perform bivariate analysis.
8. Perform multivariate analysis.
9. Detect and handle outliers.
10. Analyze feature correlations.
11. Prepare data for modeling.

## Summary

- Univariate: Explore one variable.
- Bivariate: Explore the relationship between two variables.
- Multivariate: Explore interactions among three or more variables.

## Easy Way To Remember

- Uni = 1
- Bi = 2
- Multi = 3 or more
