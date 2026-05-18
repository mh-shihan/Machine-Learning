# Tensor

A tensor is a generalization of scalars, vectors, and matrices to higher dimensions. It is a fundamental data structure in machine learning and deep learning frameworks, such as TensorFlow and PyTorch. Tensors can represent multi-dimensional arrays of data, and they support various operations like addition, multiplication, and more complex transformations.

## 1. 0-D Tensor (Scalar)

A 0-D tensor is a single value, also known as a scalar. It has no dimensions.

```python
import numpy as np
scalar = np.array(5)
print(scalar)  # Output: 5
```

## 2. 1-D Tensor (Vector)

A 1-D tensor is a one-dimensional array, also known as a vector. It has a single dimension.

```python
vector = np.array([1, 2, 3])
print(vector)  # Output: [1 2 3]
```

## 3. 2-D Tensor (Matrix)

A 2-D tensor is a two-dimensional array, also known as a matrix. It has two dimensions.

```python
matrix = np.array([[1, 2], [3, 4]])
print(matrix)  # Output: [[1 2], [3 4]]
```

## 4. N-D Tensors

An N-D tensor is a multi-dimensional array that can have any number of dimensions. For example, a 3-D tensor can be represented as follows:

```python
tensor_3d = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
print(tensor_3d)
# Output: [[[1 2], [3 4]], [[5 6], [7 8]]]
```

## Rank

The rank of a tensor refers to the number of dimensions it has. For example, a scalar has a rank of 0, a vector has a rank of 1, a matrix has a rank of 2, and so on.

```python
print(scalar.ndim)  # Output: 0
print(vector.ndim)  # Output: 1
print(matrix.ndim)  # Output: 2
print(tensor_3d.ndim)  # Output: 3
```

## Axis

The axis of a tensor refers to the specific dimension along which an operation is performed. For example, in a 2-D tensor (matrix), axis 0 refers to the rows, and axis 1 refers to the columns.

```python
print(matrix.sum(axis=0))  # Sum along columns (axis 0)
# Output: [4 6]
print(matrix.sum(axis=1))  # Sum along rows (axis 1)
# Output: [3 7]
```

## Shape

The shape of a tensor is a tuple that describes the size of each dimension. For example, the shape of a 2-D tensor (matrix) with 3 rows and 4 columns would be (3, 4).

```python
print(scalar.shape)  # Output: ()
print(vector.shape)  # Output: (3,)
print(matrix.shape)  # Output: (2, 2)
print(tensor_3d.shape)  # Output: (2, 2, 2)
```

## Size

The size of a tensor is the total number of elements it contains. It can be calculated by multiplying the dimensions together.

```python
print(scalar.size)  # Output: 1
print(vector.size)  # Output: 3
print(matrix.size)  # Output: 4
print(tensor_3d.size)  # Output: 8
```
