# Dictionaries

Dictionaries store key-value pairs.

```python
employee = {
    "id": 101,
    "name": "Ayan",
    "role": "AI Platform Engineer"
}
```

## Access and Update
```python
print(employee["name"])
print(employee.get("team"))
employee["team"] = "Platform"
```

## Looping
```python
for key, value in employee.items():
    print(key, value)
```

## Company Use
JSON-like API data, configuration, database records, lookup tables.

## Common Mistakes
- `KeyError` from missing keys
- Assuming keys are automatically normalized

## Interview Questions
1. Why use `.get()`?
2. Can dictionary keys be lists?

## Practice
Store a server record with name, region, status, CPU, and tags.