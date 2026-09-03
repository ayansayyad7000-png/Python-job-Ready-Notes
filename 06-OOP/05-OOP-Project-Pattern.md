# OOP Project Pattern

A small project can separate responsibilities across classes.

```text
monitoring_app/
├── main.py
├── models.py
├── monitor.py
└── notifier.py
```

Example design:
```python
class Server:
    def __init__(self, name, cpu):
        self.name = name
        self.cpu = cpu

class HealthChecker:
    def get_status(self, server):
        return "CRITICAL" if server.cpu >= 90 else "OK"
```

## Design Rule
A class should have one clear reason to change.

## Prefer Composition
Instead of building deep inheritance trees, combine focused objects.

```python
class MonitoringService:
    def __init__(self, checker, notifier):
        self.checker = checker
        self.notifier = notifier
```

## Practice Project
Build:
- `Employee`
- `SalaryCalculator`
- `ReportWriter`

Keep calculation and file-writing responsibilities separate.