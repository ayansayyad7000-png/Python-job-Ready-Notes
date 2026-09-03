# Virtual Environments

A virtual environment isolates project dependencies.

## Create
```bash
python -m venv .venv
```

## Activate
Windows PowerShell:
```powershell
.\.venv\Scripts\Activate.ps1
```
Linux/macOS:
```bash
source .venv/bin/activate
```

Install packages inside it:
```bash
python -m pip install requests
```

Deactivate:
```bash
deactivate
```

## Company Use
Different projects may require different package versions. Virtual environments prevent conflicts.

## Good Practice
Do not commit `.venv/` to Git. Add it to `.gitignore`.

## Interview Question
Why should each Python project have its own environment?