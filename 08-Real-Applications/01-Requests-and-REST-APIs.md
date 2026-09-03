# Requests and REST APIs

Install:
```bash
python -m pip install requests
```

## GET Request
```python
import requests

response = requests.get("https://api.example.com/items", timeout=10)
response.raise_for_status()
data = response.json()
```

## POST Request
```python
payload = {"name": "Ayan"}
response = requests.post(
    "https://api.example.com/users",
    json=payload,
    timeout=10,
)
```

## Production Habits
- Set timeouts
- Handle request errors
- Check status codes
- Validate returned data
- Never hard-code secrets

## Company Use
Service-to-service communication, automation, integrations, cloud APIs.

## Interview Questions
1. GET vs POST?
2. Why use a timeout?
3. What does `raise_for_status()` do?

## Practice
Call a public JSON API and print selected fields safely.