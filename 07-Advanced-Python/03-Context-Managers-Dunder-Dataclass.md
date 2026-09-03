# 03 — Context Managers, Dunder Methods & dataclass

## Context Manager
Resource setup/cleanup safely manage karta hai.

```python
with open("data.txt") as file:
    print(file.read())
```

`with` ke baad file automatically close.

Custom context manager usually `__enter__` / `__exit__` implement karta hai.

## Dunder Methods
Special methods like:
```text
__init__
__str__
__repr__
__len__
__eq__
```

```python
class Server:
    def __init__(self, name):
        self.name = name

    def __str__(self):
        return self.name
```

## dataclass
Boilerplate reduce:

```python
from dataclasses import dataclass

@dataclass
class Employee:
    name: str
    role: str
    salary: float = 0.0
```

Auto-generated init/repr/equality useful hain.

## Company Use
Data models, config objects, DTO-like structures.
