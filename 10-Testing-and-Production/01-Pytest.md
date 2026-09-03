# 01 — Testing with pytest

Install:
```bash
pip install pytest
```

Code:
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
pytest
```

## Arrange-Act-Assert
```python
def test_discount():
    # Arrange
    price = 100

    # Act
    result = apply_discount(price, 10)

    # Assert
    assert result == 90
```

## Exceptions
```python
import pytest

with pytest.raises(ValueError):
    set_age(-1)
```

## Fixtures
Reusable test setup:
```python
@pytest.fixture
def sample_user():
    return {"name": "Ayan"}
```

## Company Use
CI pipelines tests run karte hain before merge/deploy.
