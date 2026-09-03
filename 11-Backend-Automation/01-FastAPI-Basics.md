# 01 — FastAPI Basics

## Goal
Python se typed REST API banana.

## Install
Virtual environment ke andar:

```bash
pip install "fastapi[standard]"
```

## First API — `main.py`
```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
async def root():
    return {"message": "Hello World"}
```

Development server:
```bash
fastapi dev main.py
```

If using a `uv` managed project, FastAPI CLI can be run through `uv run`.

Open:
```text
http://127.0.0.1:8000
http://127.0.0.1:8000/docs
```

`/docs` automatic interactive Swagger UI deta hai.

## Path Parameter
```python
@app.get("/users/{user_id}")
def get_user(user_id: int):
    return {"user_id": user_id}
```

## Request Body
```python
from pydantic import BaseModel

class UserCreate(BaseModel):
    name: str
    age: int

@app.post("/users")
def create_user(user: UserCreate):
    return user
```

## Company Structure
Routes → services → database/client layers separate rakho as app grows.

## Production Thinking
Validation, auth, logging, errors, tests, config, DB connection lifecycle important hain.
