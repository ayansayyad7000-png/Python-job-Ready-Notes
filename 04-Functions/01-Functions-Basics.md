# 01 — Functions Basics

## Simple Meaning
Function reusable block of code hai.

```python
def greet():
    print("Hello")

greet()
```

`def` function define karta hai. `greet()` function call hai.

## Why Functions?
Bad:
```python
print("Checking server")
print("Checking server")
print("Checking server")
```

Better:
```python
def check_server():
    print("Checking server")

check_server()
check_server()
```

## Parameters
```python
def greet(name):
    print(f"Hello {name}")

greet("Ayan")
```

`name` parameter; `"Ayan"` argument.

## Company Use
```python
def build_s3_path(bucket, key):
    return f"s3://{bucket}/{key}"
```

Reusable small functions testing aur maintenance easy banate hain.

## Good Function Rule
Ek function ideally ek clear responsibility rakhe.

## Interview
- Function define: `def`.
- Parameter definition me; argument call me.
- Function reuse, readability, testability improve karta hai.

## Practice
1. `say_hello()`.
2. `greet(name)`.
3. `square(number)`.
4. `is_even(number)`.
