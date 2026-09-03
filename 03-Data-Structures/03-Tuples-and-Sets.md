# Tuples and Sets

## Tuple
Ordered and immutable.
```python
point = (10, 20)
```
Useful for fixed records or values that should not change.

## Set
Unordered collection of unique values.
```python
skills = {"Python", "AWS", "Python"}
print(skills)
```

Useful operations:
```python
a | b   # union
a & b   # intersection
a - b   # difference
```

## Company Use
- Tuple: fixed coordinates, configuration pairs, immutable records
- Set: remove duplicates, fast membership checks, compare permissions

## Interview Questions
1. List vs tuple?
2. Why use a set?

## Practice
Find common skills between two teams using set intersection.