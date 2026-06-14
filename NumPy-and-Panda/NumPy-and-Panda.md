# NumPy and Pandas 


### In Machine Learning:

- **NumPy** = Mathematical operations on arrays and matrices
- **Pandas** = Loading, cleaning, and analyzing datasets

Typical workflow:

```text
CSV Dataset
     ↓
Pandas
     ↓
Cleaning & Preprocessing
     ↓
NumPy Arrays
     ↓
Scikit-Learn / TensorFlow / PyTorch
     ↓
Model Training

```
## NumPy
NumPy stands for Numerical Python.

It provides a powerful data structure called:
```python
ndarray (n-dimensional array)
```
**Example of creating a NumPy array:** 
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
```

## Pandas
### Pandas is used for:
- Reading CSV files
- Data Cleaning
- Data Analysis
- Feature Engineering
```python
import pandas as pd
```
### DataFrame

A DataFrame is like an Excel sheet
```python
import pandas as pd

data = {
    "Name": ["Alice", "Bob", "Charlie"],
    "Age": [25, 30, 22]
}

df = pd.DataFrame(data)

print(df)
```

### Reading a CSV file
```python
import pandas as pd
df = pd.read_csv('data.csv')
print(df.head())
```
