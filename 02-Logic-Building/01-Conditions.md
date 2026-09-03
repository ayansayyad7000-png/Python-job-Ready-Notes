# 01 — Conditions: if, elif, else

## Simple Meaning
Condition program ko decision lene deti hai.

```python
age = 21

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

## Flow
```text
condition True? → if block
otherwise       → else block
```

## `elif`
Multiple conditions ke liye:

```python
marks = 72

if marks >= 90:
    grade = "A"
elif marks >= 75:
    grade = "B"
elif marks >= 60:
    grade = "C"
else:
    grade = "D"

print(grade)
```

## Nested Condition
```python
is_active = True
role = "admin"

if is_active:
    if role == "admin":
        print("Full access")
```

Nested logic useful hai, but bahut deep nesting avoid karo.

## Company Example
```python
status_code = 200

if 200 <= status_code < 300:
    print("Request successful")
elif status_code == 404:
    print("Resource not found")
else:
    print("Request failed")
```

## Common Mistakes
- `=` ki jagah `==` comparison me use karo.
- Colon `:` mat bhoolo.
- Indentation correct rakho.
- Conditions ka order important hai.

## Interview
**Q. `if` aur `elif` me difference?**  
`if` first condition start karta hai; `elif` additional conditions check karta hai.

**Q. Multiple `if` vs `if/elif`?**  
Multiple `if` sab independently check hote hain. `elif` chain me first true branch ke baad remaining skip hote hain.

## Practice
1. Number positive/negative/zero.
2. Age based eligibility.
3. Marks to grade.
4. Username + password simple check.
5. Environment `dev/staging/prod` message.

## Quick Revision
```text
if = first condition
elif = another condition
else = fallback
comparison = == != > < >= <=
```
