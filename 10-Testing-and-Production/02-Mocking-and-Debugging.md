# 02 — Mocking & Debugging

## Mocking
External dependency ko fake/control karna, so test network/DB par depend na ho.

```python
from unittest.mock import Mock

client = Mock()
client.get_status.return_value = "running"
assert client.get_status() == "running"
```

`pytest` + `monkeypatch` bhi common hai.

## Debugging
First tools:
```python
print(value)
```
But professional workflow:
- read traceback bottom-up
- inspect variable types/values
- reproduce smallest failing case
- debugger breakpoint use karo
- logs check karo

Built-in debugger:
```python
breakpoint()
```

## Traceback Habit
Error type + exact line identify karo before random code changes.

## Company Use
Mocks reliable tests; debugger/logs production issues diagnose karne me help.
