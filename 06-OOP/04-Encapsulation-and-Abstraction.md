# Encapsulation and Abstraction

## Encapsulation
Keep internal details behind a clear interface.

```python
class Account:
    def __init__(self, balance=0):
        self._balance = balance

    def deposit(self, amount):
        if amount <= 0:
            raise ValueError("amount must be positive")
        self._balance += amount
```

Python uses conventions such as `_name` for internal attributes.

## Abstraction
Expose what callers need while hiding implementation details.

Example: a caller uses `storage.save(data)` without knowing whether storage is local disk or S3.

## Company Use
Stable interfaces allow implementations to change without rewriting every caller.

## Common Mistakes
- Treating `_private` as strict security; it is a convention
- Exposing internal mutable state unnecessarily

## Interview Questions
1. What is encapsulation?
2. What is abstraction?