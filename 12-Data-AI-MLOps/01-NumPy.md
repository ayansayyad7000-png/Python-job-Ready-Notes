# 01 — NumPy Basics

Install:
```bash
pip install numpy
```

## Array
```python
import numpy as np

values = np.array([10, 20, 30])
print(values)
print(values.dtype)
print(values.shape)
```

## Vectorized Operations
```python
values = np.array([1, 2, 3])
print(values * 10)
```

No manual loop needed for many numeric operations.

## 2D
```python
matrix = np.array([[1, 2], [3, 4]])
print(matrix.shape)
print(matrix[:, 0])
```

## Useful
```python
np.mean(values)
np.sum(values)
np.min(values)
np.max(values)
```

## Boolean Filtering
```python
cpu = np.array([40, 92, 70, 99])
print(cpu[cpu >= 90])
```

## Company Use
Numerical processing, ML features, matrix/data operations.

## Important
NumPy arrays generally homogeneous numeric computation ke liye optimized hote hain.
