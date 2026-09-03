# 02 — Virtual Environments

## Problem
Project A ko package v1 chahiye, Project B ko v2. Global installs conflict kar sakte hain.

## Solution: venv
Create:
```bash
python -m venv .venv
```

Windows PowerShell:
```powershell
.\.venv\Scripts\Activate.ps1
```

Linux/macOS:
```bash
source .venv/bin/activate
```

Install:
```bash
pip install requests
```

Save:
```bash
pip freeze > requirements.txt
```

Deactivate:
```bash
deactivate
```

## `.gitignore`
`.venv` Git me commit nahi karna:
```text
.venv/
__pycache__/
.env
```

## Company Workflow
```text
clone repo
→ create venv
→ activate
→ pip install -r requirements.txt
→ run app/tests
```

## Interview
Virtual environment project dependencies isolate karta hai.
