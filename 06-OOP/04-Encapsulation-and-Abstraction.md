# 04 — Encapsulation & Abstraction

## Encapsulation
Internal state ko controlled methods/properties ke through manage karna.

```python
class Account:
    def __init__(self, balance=0):
        self._balance = balance

    def deposit(self, amount):
        if amount <= 0:
            raise ValueError("Amount must be positive")
        self._balance += amount
```

Python me `_name` convention means internal/protected-like use.

## Property
```python
class Account:
    def __init__(self, balance):
        self._balance = balance

    @property
    def balance(self):
        return self._balance
```

## Abstraction
User ko simple interface do, internal complexity hide karo.

Example:
```python
client.upload("report.csv")
```
Caller ko underlying HTTP/auth steps jaana zaroori nahi.

## Company Use
Service classes, SDK wrappers, repositories, API clients.

## Interview
Encapsulation state/control organize karta hai; abstraction unnecessary implementation detail hide karta hai.
