# Type Hints

Type hints document expected types and help static analysis tools.

```python
def calculate_total(price: float, quantity: int) -> float:
    return price * quantity
```

## Collections
```python
def active_names(users: list[dict[str, object]]) -> list[str]:
    return [str(u["name"]) for u in users if u.get("active")]
```

## Optional Values
```python
def find_user(user_id: int) -> dict | None:
    ...
```

## Why Companies Use Them
- Better editor support
- Easier code review
- Earlier bug detection with tools such as mypy or pyright
- Clearer API contracts

## Important
Python does not enforce most hints at runtime automatically.

## Common Mistakes
- Treating type hints as runtime validation
- Adding extremely complex types that reduce readability

## Interview Question
Do type hints change Python into a statically typed language?