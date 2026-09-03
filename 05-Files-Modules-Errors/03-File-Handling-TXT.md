# 03 — File Handling (TXT)

## Recommended: `with open()`
Read:
```python
with open("notes.txt", "r", encoding="utf-8") as file:
    content = file.read()
```

Write (overwrites):
```python
with open("notes.txt", "w", encoding="utf-8") as file:
    file.write("Python\n")
```

Append:
```python
with open("notes.txt", "a", encoding="utf-8") as file:
    file.write("AWS\n")
```

## Modes
```text
r read
w write/overwrite
a append
b binary
```

## Lines
```python
with open("notes.txt", encoding="utf-8") as file:
    for line in file:
        print(line.strip())
```

## Why `with`?
Context manager file automatically close karta hai, even if error occurs.

## Company Use
Config, logs, exported data, templates, small automation files.

## Common Mistake
`w` existing content erase karta hai. Append ke liye `a`.

## Practice
1. File write.
2. Append 3 lines.
3. Read line-by-line.
4. Count lines/words.
