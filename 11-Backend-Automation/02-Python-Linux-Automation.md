# Python + Linux Automation

Python is widely used to automate system tasks.

## Run Commands Safely
```python
import subprocess

result = subprocess.run(
    ["systemctl", "is-active", "nginx"],
    capture_output=True,
    text=True,
    check=False,
)

print(result.stdout.strip())
```

Prefer argument lists over `shell=True` for untrusted input.

## File Automation
```python
from pathlib import Path

for path in Path("/var/log").glob("*.log"):
    print(path)
```

## Environment Variables
```python
import os
region = os.getenv("AWS_REGION", "ap-south-1")
```

## Company Use
Deployment helpers, health checks, cleanup jobs, backup scripts, CI/CD utilities.

## Common Mistakes
- Building shell commands from user input
- Ignoring command exit codes
- Running scripts with unnecessary root privileges

## Interview Question
Why is `subprocess.run([...])` often safer than building a shell command string?