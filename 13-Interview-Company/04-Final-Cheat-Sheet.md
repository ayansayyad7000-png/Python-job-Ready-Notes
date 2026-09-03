# Final Python Cheat Sheet

## Variables
```python
name = "Ayan"
age = 21
```

## Condition
```python
if age >= 18:
    print("adult")
```

## Loop
```python
for item in items:
    print(item)
```

## Function
```python
def add(a, b):
    return a + b
```

## List / Dict
```python
skills = ["Python", "AWS"]
user = {"id": 1, "name": "Ayan"}
```

## Comprehension
```python
active_ids = [u["id"] for u in users if u["active"]]
```

## Exception
```python
try:
    value = int(text)
except ValueError:
    value = 0
```

## File
```python
from pathlib import Path
text = Path("data.txt").read_text(encoding="utf-8")
```

## JSON
```python
import json
data = json.loads(text)
```

## HTTP
```python
requests.get(url, timeout=10)
```

## SQL Safety
Use parameterized queries, never string-built SQL with untrusted input.

## Logging
```python
logger.info("job_id=%s started", job_id)
```

## Async
```python
async def work():
    await something()
```

## AWS
Use boto3 with IAM roles; never hard-code credentials.

## Production Checklist
```text
clear names
small functions
input validation
specific exceptions
logging
config outside code
secrets outside Git
tests
timeouts
safe SQL
clean project structure
type hints where useful
```

## Learning Order
```text
Basics → Logic → Data Structures → Functions → Files/Errors → OOP
→ Advanced Python → APIs/SQL/Testing → Backend/Cloud → Data/MLOps
→ Projects → Interview Revision
```