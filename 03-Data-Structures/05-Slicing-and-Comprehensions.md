# Slicing and Comprehensions

## Slicing
```python
values = [10, 20, 30, 40, 50]
print(values[1:4])
print(values[::-1])
```
Format:
```text
sequence[start:stop:step]
```
`stop` is excluded.

## List Comprehension
```python
squares = [n * n for n in range(5)]
```
With a condition:
```python
high_cpu = [x for x in cpu_values if x >= 80]
```

## Dictionary Comprehension
```python
mapping = {n: n * n for n in range(5)}
```

## Company Use
Filtering and transforming small-to-medium collections clearly.

## Common Mistakes
- Overly complex comprehensions
- Forgetting slicing stop is exclusive

## Interview Question
When is a normal loop clearer than a comprehension?

## Practice
Create a list containing only active user IDs from a list of user dictionaries.