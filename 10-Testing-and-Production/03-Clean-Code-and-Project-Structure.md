# Clean Code and Project Structure

## Principles
- Clear names
- Small focused functions
- One responsibility per module
- Explicit error handling
- Minimal duplication
- Useful type hints
- Tests for important behavior

## Example Structure
```text
project/
├── pyproject.toml
├── README.md
├── src/
│   └── app/
│       ├── __init__.py
│       ├── main.py
│       ├── config.py
│       └── services.py
└── tests/
    └── test_services.py
```

## Dependency Files
Modern projects often use `pyproject.toml`; some still use `requirements.txt`.

## PEP 8
PEP 8 is Python's style guide. Automated formatters and linters help enforce consistency.

## Company Use
Good structure makes onboarding, testing, deployment, and ownership easier.

## Common Mistakes
- Huge `main.py`
- Business logic mixed with database/network code
- Secrets committed to Git

## Interview Question
What makes code maintainable?