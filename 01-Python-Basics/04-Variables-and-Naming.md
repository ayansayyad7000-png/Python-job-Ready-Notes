# 04 — Variables and Naming

A variable is a name that refers to a value.

```python
name = "Ayan"
age = 21
salary = 50000.0
is_active = True
```

## Naming Rules
Valid:
```python
user_name = "Ayan"
retry_count = 3
```
Invalid:
```text
2name
user-name
class
```

## Good Style
Use `snake_case` for variables and functions.

```python
monthly_salary = 50000
```
Use uppercase for constants by convention:
```python
MAX_RETRIES = 3
```

## Multiple Assignment
```python
x, y = 10, 20
```

## Company Use
Clear variable names reduce bugs and make pull requests easier to review.

## Common Mistakes
- Reusing built-in names such as `list`, `str`, `id`
- Using unclear abbreviations
- Treating constants as truly immutable; uppercase is only a convention

## Interview Questions
1. Does Python require variable type declarations?
2. What naming style is recommended?

## Practice
Create variables for employee ID, name, salary, role, and active status.