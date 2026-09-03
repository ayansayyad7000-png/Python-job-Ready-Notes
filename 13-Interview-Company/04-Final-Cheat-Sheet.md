# 04 — Python Final Cheat Sheet

```python
# variables
name = "Ayan"
age = 21

# collections
items = [1, 2]
fixed = (1, 2)
unique = {1, 2}
user = {"name": "Ayan"}

# condition
if age >= 18:
    pass
elif age == 17:
    pass
else:
    pass

# loop
for item in items:
    print(item)

# function
def add(a: int, b: int = 0) -> int:
    return a + b

# comprehension
evens = [n for n in range(10) if n % 2 == 0]

# exceptions
try:
    value = int("10")
except ValueError:
    value = 0

# file
with open("data.txt", encoding="utf-8") as file:
    content = file.read()

# class
class User:
    def __init__(self, name):
        self.name = name

# generator
def numbers():
    yield 1

# async
import asyncio
async def main():
    await asyncio.sleep(1)

# logging
import logging
logger = logging.getLogger(__name__)

# env
import os
api_key = os.getenv("API_KEY")
```

## Production Checklist
- virtual environment
- dependencies pinned/managed
- config outside code
- no secrets in Git
- type hints where helpful
- specific exceptions
- logging
- tests
- clean functions/classes
- README setup instructions
- database queries parameterized
- API timeouts
- code review friendly naming

## Interview Answer Formula
```text
Definition → Example → Real use → Important edge case/tradeoff
```
