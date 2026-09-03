# Conditions: if, elif, else

Conditions run code only when a rule is true.

```python
score = 82

if score >= 90:
    grade = "A"
elif score >= 75:
    grade = "B"
else:
    grade = "C"

print(grade)
```

## Multiple Conditions
```python
if is_active and role == "admin":
    print("Access granted")
```

## Company Use
Permissions, validation, pricing rules, retries, feature flags, and workflow decisions.

## Common Mistakes
- Incorrect condition order
- Deeply nested `if` blocks
- Using `== True` unnecessarily

## Interview Questions
1. When should `elif` be used?
2. What is short-circuit evaluation?

## Practice
Build a login decision using username, password status, and account-active status.