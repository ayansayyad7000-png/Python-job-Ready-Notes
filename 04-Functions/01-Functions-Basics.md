# Functions Basics

Functions group reusable logic.

```python
def greet(name):
    print(f"Hello, {name}")

greet("Ayan")
```

## Why Functions Matter
- Reduce repeated code
- Make testing easier
- Improve readability
- Separate responsibilities

## Good Function Design
Prefer small functions with one clear purpose.

```python
def calculate_total(price, quantity):
    return price * quantity
```

## Company Use
Validation helpers, API logic, calculations, file processing, automation tasks.

## Common Mistakes
- Functions that do too many unrelated tasks
- Hidden global-state changes
- Poor names such as `do_it()`

## Interview Questions
1. Why use functions?
2. What is the difference between defining and calling a function?

## Practice
Write functions for tax calculation, email validation, and checking server health.