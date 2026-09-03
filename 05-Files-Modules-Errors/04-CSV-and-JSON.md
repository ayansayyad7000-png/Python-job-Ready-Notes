# 04 — CSV & JSON

# CSV
```python
import csv

with open("employees.csv", "r", newline="", encoding="utf-8") as file:
    reader = csv.DictReader(file)
    for row in reader:
        print(row["name"])
```

Write:
```python
import csv

rows = [{"name": "Ayan", "role": "Platform"}]
with open("employees.csv", "w", newline="", encoding="utf-8") as file:
    writer = csv.DictWriter(file, fieldnames=["name", "role"])
    writer.writeheader()
    writer.writerows(rows)
```

# JSON
```python
import json

employee = {"name": "Ayan", "skills": ["Python", "AWS"]}

with open("employee.json", "w", encoding="utf-8") as file:
    json.dump(employee, file, indent=2)
```

Read:
```python
with open("employee.json", encoding="utf-8") as file:
    data = json.load(file)
```

## Important
- `json.load()` file → Python.
- `json.loads()` string → Python.
- `json.dump()` Python → file.
- `json.dumps()` Python → string.

## Company Use
APIs mostly JSON; exports/imports me CSV common.

## Interview
CSV tabular; JSON nested structured data better handle karta hai.
