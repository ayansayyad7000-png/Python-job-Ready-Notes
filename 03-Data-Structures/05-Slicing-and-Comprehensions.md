# 05 — Slicing & Comprehensions

# Slicing
Syntax:
```python
sequence[start:stop:step]
```

Example:
```python
marks = [20, 40, 60, 80, 100]

print(marks[1:4])
print(marks[:3])
print(marks[2:])
print(marks[::-1])
```

Important: stop index exclude hota hai.

Negative direction:
```python
print(marks[-1:-3:-1])
```

Default step `+1` hota hai, so reverse slice ke liye negative step chahiye.

# List Comprehension
Normal:
```python
squares = []
for n in range(1, 6):
    squares.append(n * n)
```

Comprehension:
```python
squares = [n * n for n in range(1, 6)]
```

With condition:
```python
evens = [n for n in range(1, 11) if n % 2 == 0]
```

# Dict Comprehension
```python
squares = {n: n * n for n in range(1, 5)}
```

## Company Rule
Comprehension concise ho, but unreadable one-liner mat banao. Complex logic normal loop me better hota hai.

## Interview
- slicing stop exclusive.
- `[::-1]` reverse.
- comprehension compact transformation/filtering.

## Practice
1. Last 3 items slice.
2. Reverse list.
3. Even numbers comprehension.
4. Names lowercase comprehension.
5. Dict number→square.
