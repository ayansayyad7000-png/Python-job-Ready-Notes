# Context Managers, Dunder Methods and dataclass

## Context Manager
`with` manages setup and cleanup.

```python
with open("data.txt", encoding="utf-8") as file:
    data = file.read()
```

Custom context managers can implement `__enter__` and `__exit__`.

## Dunder Methods
Special methods such as `__str__`, `__len__`, and `__eq__` integrate objects with Python syntax.

```python
class Service:
    def __init__(self, name):
        self.name = name

    def __str__(self):
        return self.name
```

## dataclass
Useful for data-focused classes.

```python
from dataclasses import dataclass

@dataclass
class Server:
    name: str
    cpu: float
```

## Company Use
Resource management, domain records, clean model objects.

## Interview Questions
1. Why use a context manager?
2. When is `dataclass` useful?

## Practice
Create a `Deployment` dataclass with service, version, and environment.