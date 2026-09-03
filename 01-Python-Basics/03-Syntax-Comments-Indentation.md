# 03 — Syntax, Comments and Indentation

## Statements
```python
name = "Ayan"
print(name)
```

## Comments
```python
# This is a comment
```
Use comments to explain *why*, not obvious code.

## Indentation
Python uses indentation to define blocks.

```python
age = 21
if age >= 18:
    print("Adult")
```

Wrong indentation can raise `IndentationError`.

## Naming Style
Prefer readable names:
```python
user_count = 10
is_active = True
```

## Company Use
Consistent formatting makes code easier to review and maintain in teams.

## Common Mistakes
- Mixing tabs and spaces
- Forgetting `:` after `if`, `for`, `while`, `def`, `class`
- Poor variable names such as `x1`, `abc`, `tmp2`

## Interview Questions
1. Why is indentation important in Python?
2. What does `#` do?

## Practice
Write an `if` block with correct indentation and add one useful comment.