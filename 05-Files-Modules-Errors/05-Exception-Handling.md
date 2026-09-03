# 05 — Exception Handling

## Problem
Bad input program crash kar sakta hai.

```python
number = int("abc")
```
Raises `ValueError`.

## try/except
```python
try:
    age = int(input("Age: "))
except ValueError:
    print("Enter a valid number")
```

## else/finally
```python
try:
    value = int("10")
except ValueError:
    print("Invalid")
else:
    print("Success", value)
finally:
    print("Finished")
```

- `else` only if no exception.
- `finally` always runs.

## Catch Specific Exceptions
Good:
```python
except FileNotFoundError:
    ...
```

Avoid broad silent handling:
```python
except Exception:
    pass
```

## Raise
```python
def set_age(age):
    if age < 0:
        raise ValueError("Age cannot be negative")
```

## Company Use
API, file, database, network calls fail ho sakte hain. Graceful handling + logging important hai.

## Interview
- Exception runtime error/event hai.
- Specific exceptions catch karo.
- `finally` cleanup ke liye useful.

## Practice
1. Safe integer input.
2. File not found handle.
3. Division by zero handle.
4. Negative salary par raise.
