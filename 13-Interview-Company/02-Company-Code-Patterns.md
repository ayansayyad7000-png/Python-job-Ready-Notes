# Company-Style Python Patterns

## 1. Validate Inputs Early
```python
def create_user(name: str) -> dict:
    clean_name = name.strip()
    if not clean_name:
        raise ValueError("name is required")
    return {"name": clean_name}
```

## 2. Keep Configuration Outside Business Logic
```python
API_URL = os.getenv("API_URL")
```

## 3. Use Small Service Functions
```python
def calculate_total(items):
    return sum(item["price"] for item in items)
```

## 4. Handle External Failures
Network, database, cloud, and file operations can fail. Add timeouts, clear exceptions, retries only where appropriate, and useful logs.

## 5. Keep Secrets Out of Git
Use environment variables, IAM roles, or secret managers.

## 6. Write Tests Around Important Behavior
Test business rules and error cases, not only happy paths.

## 7. Separate Layers
```text
API / CLI
→ service logic
→ data/cloud clients
→ external systems
```

## 8. Make Operations Observable
Use logs, metrics, health checks, and meaningful error messages.

## Review Checklist
- Clear names?
- Inputs validated?
- Errors handled?
- Secrets protected?
- Tests present?
- Function too large?
- External dependency isolated?