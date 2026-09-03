# 05 — Data Types

## Core Types
```python
name = "Ayan"            # str
age = 21                  # int
salary = 50000.50         # float
is_active = True          # bool
skills = ["Python"]      # list
coordinates = (10, 20)    # tuple
tags = {"aws", "python"} # set
user = {"id": 101}       # dict
manager = None            # NoneType
```

Check a type:
```python
print(type(age))
```

## Mutable vs Immutable
Common mutable types: `list`, `dict`, `set`.
Common immutable types: `int`, `float`, `str`, `tuple`, `bool`.

## Company Use
Choosing the correct type improves clarity and reduces unnecessary conversions.

## Common Mistakes
- Mixing numbers and strings without conversion
- Expecting tuples or strings to change in place
- Using a list when uniqueness is required; a set may be better

## Interview Questions
1. List vs tuple?
2. What does `None` mean?
3. Which common built-in types are mutable?

## Practice
Create one variable for each core type and print its value and type.