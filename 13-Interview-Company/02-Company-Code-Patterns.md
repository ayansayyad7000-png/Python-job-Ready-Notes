# 02 — Company-Style Python Patterns

## Pattern 1 — Validate Early
```python
def create_user(name: str) -> dict:
    clean_name = name.strip()
    if not clean_name:
        raise ValueError("name is required")
    return {"name": clean_name}
```

## Pattern 2 — Separate Config
```python
import os
API_URL = os.getenv("API_URL", "http://localhost:8000")
```

## Pattern 3 — Specific Errors
Catch expected exceptions, log context, don't silently ignore.

## Pattern 4 — Small Layers
```text
route/controller
→ service/business logic
→ repository/client
→ external DB/API
```

## Pattern 5 — Dependency Injection Idea
Function/class ko dependency parameter me do instead of globally create karna. Testing easy hota hai.

```python
def get_status(client, server_id):
    return client.fetch_status(server_id)
```

## Pattern 6 — Return Data, Don't Randomly Print
Business functions result return kare; UI/CLI layer display kare.

## Pattern 7 — Logging
Important actions/errors log; secrets never log.

## Pattern 8 — Tests for Behavior
Happy path + invalid input + edge cases.

## Pattern 9 — Idempotency Thinking
Automation ko repeat run karne par unexpected duplicate/damage na ho where possible.

## Pattern 10 — Readability
Clever one-liners se better clear code.
