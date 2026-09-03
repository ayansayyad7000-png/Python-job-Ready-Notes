# 03 — Clean Code & Project Structure

## Naming
```python
monthly_salary = 50000
```
Better than:
```python
ms = 50000
```

## Small Functions
One clear responsibility.

## Avoid Magic Numbers
Bad:
```python
if retries > 3:
```
Better:
```python
MAX_RETRIES = 3
if retries > MAX_RETRIES:
```

## Typical Project
```text
project/
├── src/
│   └── app/
│       ├── __init__.py
│       ├── main.py
│       ├── services.py
│       └── config.py
├── tests/
├── requirements.txt
├── .gitignore
└── README.md
```

## PEP 8
Python style conventions: readable spacing, naming, line organization.

## Tools
```text
ruff   linting
black  formatting
pytest testing
mypy   type checking
```

## Company Mindset
Readable code > clever code. Handle errors, add tests, document public behavior, don't commit secrets.
