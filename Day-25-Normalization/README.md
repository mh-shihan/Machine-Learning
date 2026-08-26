# Normalization
Normalization is a technique often applied as part of data preparation for machine learning. The goal of normalization is to change the values of numeric columns in the dataset to a common scale, without distorting differences in the ranges of values.

## Why Normalization Matters
- **Speeds up training:** Optimization algorithms (like Gradient Descent) find the correct solution much faster when the data landscape is uniform.
- **Prevents math errors:** It stops numbers from exploding into massive values that overload computer memory.
- **Removes bias:** It ensures features with inherently larger units (like income in dollars vs. age in years) do not overpower the model.

## Formulas for Normalization
1. **Min-Max Normalization**:
   - Formula: X_norm = (X - X_min) / (X_max - X_min)
   - Scales the data to a fixed range, usually 0 to 1.

2. **Mean Normalization**:
   - Formula: X_norm = (X - X_mean) / (X_max - X_min)
   - Centers the data around zero and scales it to a fixed range.

3. **Max absolute Scaling**:
   - Formula: X_norm = X / X_max
   - Scales the data by its maximum absolute value.

4. **Robust Scaling**:
   - Formula: X_norm = (X - X_median) / (Q3 - Q1)
   - Centers the data around the median and scales it by the interquartile range.

## Types of Normalization
- Min-Max Normalization
- Mean Normalization
- Max absolute Scaling
- Robust Scaling