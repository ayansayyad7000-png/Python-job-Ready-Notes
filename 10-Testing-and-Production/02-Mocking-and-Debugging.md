# Mocking and Debugging

## Mocking
Replace external dependencies during a test.

```python
from unittest.mock import Mock

client = Mock()
client.get_user.return_value = {"id": 1}
```

Mock network calls, cloud SDKs, email services, or slow dependencies when appropriate.

## Debugging
Useful tools:
```python
print(variable)          # quick local check
breakpoint()             # built-in debugger
```
Also use IDE breakpoints, logs, stack traces, and focused tests.

## Company Habit
Reproduce the bug first, isolate the smallest failing case, then fix and add a regression test.

## Common Mistakes
- Mocking everything, producing unrealistic tests
- Ignoring the full exception traceback

## Interview Questions
1. Why mock an external API?
2. What is a regression test?