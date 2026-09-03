# 08 — Type Conversion

Convert values when data arrives in the wrong type.

```python
age_text = "21"
age = int(age_text)

price = float("99.50")
count = str(10)
```

## Boolean Conversion
```python
print(bool(0))      # False
print(bool(1))      # True
print(bool(""))     # False
print(bool("0"))    # True
```
A non-empty string is truthy even if its text is `"False"` or `"0"`.

## Safe Conversion
```python
value = input("Enter age: ")
try:
    age = int(value)
except ValueError:
    print("Please enter a valid integer")
```

## Company Use
APIs, environment variables, CSV files, form data, and CLI arguments often arrive as strings.

## Common Mistakes
- Calling `int("10.5")`
- Assuming `bool("False")` is false

## Interview Questions
1. Why is type conversion needed?
2. What exception can invalid `int()` conversion raise?

## Practice
Read monthly salary as input and calculate annual salary.