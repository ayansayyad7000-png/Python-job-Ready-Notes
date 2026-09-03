# FastAPI Basics

FastAPI is a modern framework for building APIs with Python type hints.

Install:
```bash
python -m pip install "fastapi[standard]"
```

`main.py`:
```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/health")
def health():
    return {"status": "ok"}
```

Run:
```bash
fastapi dev main.py
```

Open:
```text
http://127.0.0.1:8000/health
http://127.0.0.1:8000/docs
```

## Request Data
```python
from pydantic import BaseModel

class User(BaseModel):
    name: str
    age: int

@app.post("/users")
def create_user(user: User):
    return user
```

## Company Use
Internal services, model-serving APIs, backend systems, platform tooling.

## Common Mistakes
- Putting all business logic inside route functions
- No input validation
- Blocking work inside async endpoints

## Interview Questions
1. Why is FastAPI popular?
2. What does Pydantic provide?
3. What is automatic API documentation?