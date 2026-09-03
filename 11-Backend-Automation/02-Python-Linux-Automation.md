# 02 — Python + Linux Automation

## pathlib
```python
from pathlib import Path

for file in Path("logs").glob("*.log"):
    print(file)
```

## subprocess
External command safely run:
```python
import subprocess

result = subprocess.run(
    ["python", "--version"],
    capture_output=True,
    text=True,
    check=True,
)
print(result.stdout or result.stderr)
```

Prefer argument list over `shell=True` for untrusted input.

## Environment
```python
import os
region = os.getenv("AWS_REGION")
```

## Automation Pattern
```text
read config
→ validate
→ perform task
→ handle exception
→ log result
→ return exit status
```

## Example: Old Log Finder
```python
from pathlib import Path

for path in Path("logs").glob("*.log"):
    if path.stat().st_size == 0:
        print(f"Empty log: {path}")
```

## Company Use
CI utilities, deployment helpers, file cleanup, health checks, data movement.
