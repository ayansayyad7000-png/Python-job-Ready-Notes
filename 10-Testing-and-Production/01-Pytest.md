# pytest

Install:
```bash
python -m pip install pytest
```

Function:
```python
def add(a, b):
    return a + b
```

Test:
```python
def test_add():
    assert add(2, 3) == 5
```

Run:
```bash
pytest -q
```

## Fixtures
Fixtures prepare reusable test data or resources.

```python
import pytest

@pytest.fixture
def user():
    return {"id": 1, "active": True}
```

## Company Use
Regression prevention, CI/CD gates, safe refactoring.

## Good Tests
- Fast
- Independent
- Clear
- Deterministic

## Common Mistakes
- Testing implementation details instead of behavior
- Tests that depend on execution order

## Interview Question
Unit test vs integration test?