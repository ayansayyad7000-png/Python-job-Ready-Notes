# 02 — Arguments & return

## `return`
Function se value bahar bhejne ke liye:

```python
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
```

`print()` sirf display karta hai; `return` result reuse karne deta hai.

## Positional Arguments
```python
def employee(name, role):
    print(name, role)

employee("Ayan", "Platform")
```

## Keyword Arguments
```python
employee(role="Platform", name="Ayan")
```

## Default Arguments
```python
def connect(region="ap-south-1"):
    return region
```

## Multiple Return Values
```python
def stats(numbers):
    return min(numbers), max(numbers)

low, high = stats([4, 8, 2])
```

Python actually tuple return karta hai.

## Company Example
```python
def calculate_total(price, quantity, tax_rate=0.18):
    subtotal = price * quantity
    tax = subtotal * tax_rate
    return subtotal + tax
```

## Interview
**`print` vs `return`?** Display vs reusable function result.

**Default argument?** Caller value na de to default use hota hai.

## Practice
1. Calculator functions.
2. Salary annualizer.
3. Celsius→Fahrenheit.
4. Function returning min/max.
