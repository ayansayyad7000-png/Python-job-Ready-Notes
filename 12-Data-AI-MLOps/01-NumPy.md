# NumPy Basics

NumPy provides fast numerical arrays and vectorized operations.

Install:
```bash
python -m pip install numpy
```

```python
import numpy as np

values = np.array([10, 20, 30, 40])
print(values.mean())
print(values * 2)
```

## Shapes
```python
matrix = np.array([[1, 2], [3, 4]])
print(matrix.shape)
```

## Boolean Filtering
```python
high = values[values >= 30]
```

## Why NumPy Matters
Operations on arrays are usually clearer and faster than Python loops for numerical workloads.

## Company Use
Feature processing, scientific computing, ML preprocessing, metrics calculations.

## Common Mistakes
- Confusing element-wise multiplication with matrix multiplication
- Ignoring array shapes and broadcasting rules

## Interview Questions
1. Why use NumPy instead of plain lists for numeric arrays?
2. What is broadcasting?