# CSV and JSON

## JSON
Common for APIs and configuration.

```python
import json

data = {"service": "api", "status": "ok"}

with open("data.json", "w", encoding="utf-8") as file:
    json.dump(data, file, indent=2)
```

Read:
```python
with open("data.json", encoding="utf-8") as file:
    data = json.load(file)
```

## CSV
```python
import csv

with open("users.csv", newline="", encoding="utf-8") as file:
    reader = csv.DictReader(file)
    for row in reader:
        print(row)
```

## Company Use
JSON: APIs, configs, events. CSV: reports, exports, datasets.

## Common Mistakes
- Confusing JSON text with a Python dictionary
- Ignoring malformed rows
- Loading huge files into memory unnecessarily

## Interview Question
`json.load()` vs `json.loads()`?