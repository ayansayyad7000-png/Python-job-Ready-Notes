# 04 — Type Hints

## Simple Meaning
Type hints code ka expected data type document karte hain.

```python
def add(a: int, b: int) -> int:
    return a + b
```

Python runtime automatically enforce nahi karta, but IDE/static tools help karte hain.

## Common Types
```python
names: list[str] = ["Ayan"]
config: dict[str, str] = {"region": "ap-south-1"}
```

Optional:
```python
def find_user(user_id: int) -> str | None:
    ...
```

## Typed Collections / Models
```python
from dataclasses import dataclass

@dataclass
class Server:
    name: str
    cpu: float
```

## Tools
Static type checker example: `mypy` / IDE analysis.

## Company Use
Large codebase readability, refactoring safety, API contracts.

## Interview
Type hints annotations hain; Python dynamic language hi rehta hai.
