# Seaborn

Seaborn is a Python data visualization library built on top of Matplotlib that makes it easy to create statistical graphics. It integrates closely with pandas DataFrames and provides a high-level interface for drawing attractive and informative statistical plots.

## What is Seaborn?

Seaborn is a library that simplifies the creation of statistical visualizations. It extends Matplotlib's capabilities by providing:

- Built-in themes and color palettes
- Statistical estimation and plotting functions
- Dataset-oriented API (works directly with DataFrames)
- Multi-plot grids for comparing subsets of data
- Functions for visualizing univariate and bivariate distributions

## Where is Seaborn Used?

Seaborn is commonly used in:

1. **Exploratory Data Analysis (EDA)** — Understanding data distributions and relationships
2. **Statistical Visualization** — Creating plots that show statistical properties
3. **Machine Learning Workflows** — Visualizing feature distributions and correlations
4. **Data Analysis Reports** — Creating publication-quality figures
5. **Business Intelligence** — Presenting data insights visually

## Why Seaborn?

### Advantages over Matplotlib

| Aspect | Matplotlib | Seaborn |
| --- | --- | --- |
| **API** | Low-level, verbose | High-level, concise |
| **Aesthetics** | Basic styling | Beautiful themes included |
| **Statistical Plots** | Manual calculation needed | Built-in statistical estimation |
| **DataFrame Integration** | Limited | Seamless |
| **Color Palettes** | Limited options | Many professional palettes |

### Key Benefits

- **Simplified API** — Less code to create complex visualizations
- **Statistical Estimation** — Automatic calculation of means, confidence intervals, regression lines
- **Beautiful Defaults** — Professional-looking plots without customization
- **DataFrame-Friendly** — Direct support for pandas Series and DataFrames
- **Multi-plot Grids** — Easily create faceted plots for comparing groups

## Code Examples

### 1. Basic Setup and Data Loading

```python
import seaborn as sns
import pandas as pd
import matplotlib.pyplot as plt

# Load a built-in dataset
tips = sns.load_dataset('tips')

# Display first few rows
print(tips.head())
```

### 2. Distribution Plot (Univariate Analysis)

```python
# Histogram with KDE (Kernel Density Estimation)
sns.histplot(data=tips, x='total_bill', kde=True, bins=20)
plt.title('Distribution of Total Bill Amount')
plt.show()
```

### 3. Relational Plot (Bivariate Analysis)

```python
# Scatter plot showing relationship between two variables
sns.scatterplot(data=tips, x='total_bill', y='tip', hue='sex', size='party_size')
plt.title('Relationship between Total Bill and Tip')
plt.show()
```

### 4. Categorical Plot

```python
# Box plot comparing distributions across categories
sns.boxplot(data=tips, x='day', y='total_bill', hue='sex')
plt.title('Total Bill Distribution by Day and Gender')
plt.show()
```

### 5. Violin Plot (Combined Distribution and Box Plot)

```python
# Shows distribution shape along with quartiles
sns.violinplot(data=tips, x='day', y='total_bill', hue='sex')
plt.title('Distribution of Total Bill by Day and Gender')
plt.show()
```

### 6. Correlation Heatmap (Multivariate Analysis)

```python
# Calculate correlation matrix
correlation_matrix = tips.corr(numeric_only=True)

# Create heatmap
sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm', center=0)
plt.title('Correlation Matrix Heatmap')
plt.show()
```

### 7. Pair Plot (Multivariate Analysis)

```python
# Create a grid of scatter plots for all numeric variables
sns.pairplot(tips, hue='sex', diag_kind='kde')
plt.show()
```

### 8. Count Plot (Categorical Data)

```python
# Bar plot showing counts of categorical values
sns.countplot(data=tips, x='day', hue='sex')
plt.title('Count of Records by Day and Gender')
plt.show()
```

### 9. Regression Plot with Confidence Interval

```python
# Scatter plot with fitted regression line and confidence band
sns.regplot(data=tips, x='total_bill', y='tip', scatter_kws={'alpha': 0.5})
plt.title('Linear Regression: Total Bill vs Tip')
plt.show()
```

### 10. Setting Themes and Palettes

```python
# Set a theme (darkgrid, whitegrid, dark, white, ticks)
sns.set_theme(style='whitegrid', palette='husl')

# Create a plot with the new theme
sns.scatterplot(data=tips, x='total_bill', y='tip', hue='day')
plt.show()
```

## Common Seaborn Plot Types

| Plot Type | Use Case | Function |
| --- | --- | --- |
| **Histogram** | Single variable distribution | `histplot()` |
| **KDE Plot** | Smooth distribution curve | `kdeplot()` |
| **Box Plot** | Categorical vs numerical | `boxplot()` |
| **Violin Plot** | Distribution + box plot | `violinplot()` |
| **Scatter Plot** | Two numerical variables | `scatterplot()` |
| **Line Plot** | Trends over time | `lineplot()` |
| **Bar Plot** | Categorical values | `barplot()` |
| **Count Plot** | Category frequencies | `countplot()` |
| **Heatmap** | 2D numerical data | `heatmap()` |
| **Pair Plot** | All variable combinations | `pairplot()` |
| **Regression Plot** | With fitted line | `regplot()` |

## Summary

- **What:** Seaborn is a statistical visualization library built on Matplotlib for Python
- **Where:** EDA, ML workflows, data analysis, reporting
- **Why:** Simpler API, beautiful defaults, statistical estimation, DataFrame integration
- **When to Use:** When creating statistical plots from pandas DataFrames with minimal code
- **Key Strength:** Makes it easy to create publication-quality statistical visualizations

Seaborn is essential for the Exploratory Data Analysis (EDA) workflow introduced in Day-11, providing tools to visualize univariate, bivariate, and multivariate relationships in your data before building machine learning models.
