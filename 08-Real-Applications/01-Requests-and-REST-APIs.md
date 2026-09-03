# 01 — Requests & REST APIs

## HTTP Basics
Common methods:
```text
GET    read
POST   create/send
PUT    replace
PATCH  partial update
DELETE remove
```

Install:
```bash
pip install requests
```

GET:
```python
import requests

response = requests.get("https://api.example.com/users", timeout=10)
response.raise_for_status()
data = response.json()
```

POST:
```python
payload = {"name": "Ayan"}
response = requests.post("https://api.example.com/users", json=payload, timeout=10)
```

## Important Production Habits
- always use timeout
- check status/errors
- don't hardcode secrets
- validate response fields

```python
try:
    response = requests.get(url, timeout=10)
    response.raise_for_status()
except requests.RequestException as exc:
    print(f"Request failed: {exc}")
```

## Status Codes
`2xx` success, `4xx` client issue, `5xx` server issue.

## Company Use
Internal services, SaaS APIs, automation, model endpoints.
