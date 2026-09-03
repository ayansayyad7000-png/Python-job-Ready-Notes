# Decorators and Closures

## Closure
A nested function can remember values from its enclosing scope.

```python
def multiplier(factor):
    def multiply(value):
        return value * factor
    return multiply

double = multiplier(2)
```

## Decorator
A decorator wraps a function to add behavior.

```python
from functools import wraps

def log_call(func):
    @wraps(func)
    def wrapper(*args, **kwargs):
        print(f"Calling {func.__name__}")
        return func(*args, **kwargs)
    return wrapper

@log_call
def process():
    return "done"
```

## Company Use
Authentication, logging, timing, caching, retries, framework routing.

## Common Mistakes
- Forgetting `functools.wraps`
- Hiding too much behavior inside decorators

## Interview Questions
1. What is a closure?
2. What does a decorator return?

## Practice
Create a decorator that prints execution time.