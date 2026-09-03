# Exception Handling

Exceptions represent runtime errors that can be handled.

```python
try:
    age = int(input("Age: "))
except ValueError:
    print("Invalid age")
```

## else and finally
```python
try:
    result = 10 / 2
except ZeroDivisionError:
    print("Cannot divide by zero")
else:
    print(result)
finally:
    print("Finished")
```

## Raise Your Own Error
```python
def set_percentage(value):
    if not 0 <= value <= 100:
        raise ValueError("percentage must be between 0 and 100")
```

## Company Use
APIs, database operations, file access, network requests, input validation.

## Common Mistakes
- `except Exception: pass`
- Hiding errors instead of logging or handling them
- Catching exceptions too broadly

## Interview Questions
1. `try` / `except` / `else` / `finally` roles?
2. When should you raise an exception?