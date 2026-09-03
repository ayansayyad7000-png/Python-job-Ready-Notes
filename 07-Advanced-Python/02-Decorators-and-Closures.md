# 02 — Decorators & Closures

## Closure
Inner function outer variable remember kar sakta hai.

```python
def multiplier(factor):
    def multiply(value):
        return value * factor
    return multiply

double = multiplier(2)
print(double(5))
```

## Decorator
Function ko wrap karke behavior add karta hai.

```python
def log_call(func):
    def wrapper(*args, **kwargs):
        print(f"Calling {func.__name__}")
        return func(*args, **kwargs)
    return wrapper

@log_call
def add(a, b):
    return a + b
```

Better metadata preserve:
```python
from functools import wraps

@wraps(func)
def wrapper(...):
    ...
```

## Company Use
Logging, authentication, timing, retries, caching, API frameworks.

## Interview
Decorator callable ko wrap/modify karta hai without original function body changing.
