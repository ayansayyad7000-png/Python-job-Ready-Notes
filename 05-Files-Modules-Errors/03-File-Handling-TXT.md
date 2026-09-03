# Text File Handling

Use `with` so files close automatically.

## Write
```python
with open("report.txt", "w", encoding="utf-8") as file:
    file.write("System healthy\n")
```

## Read
```python
with open("report.txt", "r", encoding="utf-8") as file:
    content = file.read()
```

## Append
```python
with open("app.log", "a", encoding="utf-8") as file:
    file.write("New event\n")
```

## Company Use
Configuration files, exports, simple reports, logs, batch input.

## Common Mistakes
- Using `w` and accidentally overwriting data
- Forgetting encoding
- Hard-coding fragile file paths

## Interview Question
Why is `with open(...)` preferred?

## Practice
Create a script that appends one timestamped status line to a text file.