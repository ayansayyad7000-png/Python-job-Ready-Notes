# 04 — Dictionaries

## Simple Meaning
Dictionary key-value data structure hai.

```python
employee = {
    "id": 101,
    "name": "Ayan",
    "role": "AI Platform Engineer",
}
```

## Access
```python
print(employee["name"])
print(employee.get("role"))
```

`get()` missing key par error ke badle `None`/default de sakta hai:
```python
print(employee.get("manager", "Not assigned"))
```

## Add / Update
```python
employee["salary"] = 55000
employee["role"] = "Platform Engineer"
```

## Remove
```python
employee.pop("salary")
```

## Loop
```python
for key, value in employee.items():
    print(key, value)
```

Useful:
```python
employee.keys()
employee.values()
employee.items()
```

## Nested Dictionary
```python
server = {
    "name": "api-1",
    "metrics": {
        "cpu": 60,
        "memory": 70,
    },
}

print(server["metrics"]["cpu"])
```

## Company Use
JSON/API objects Python me commonly dictionaries ban jate hain.

## Interview
- Keys unique hoti hain.
- `dict[key]` missing key par `KeyError`.
- `dict.get(key)` safer optional lookup.

## Practice
1. Employee dict.
2. Nested server metrics.
3. All key/value print.
4. Missing key `.get()` se handle.
5. Salary update/remove.
