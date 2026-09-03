# 06 — Input and Output

## Output
```python
print("Hello")
```

## Input
```python
name = input("Enter your name: ")
print(name)
```
`input()` always returns a string.

## Numeric Input
```python
age = int(input("Age: "))
salary = float(input("Salary: "))
```

## f-Strings
```python
name = "Ayan"
age = 21
print(f"{name} is {age} years old")
```

Formatting:
```python
price = 1234.5
print(f"Price: {price:.2f}")
```

## Company Use
CLI tools, scripts, logs, reports, and debugging all depend on clear input/output handling.

## Common Mistakes
- Forgetting conversion before arithmetic
- Printing secrets or passwords in logs

## Interview Question
What type does `input()` return?

## Practice
Ask for a product name, price, and quantity, then print the total.