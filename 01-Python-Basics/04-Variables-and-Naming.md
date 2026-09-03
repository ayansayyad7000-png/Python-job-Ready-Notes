# 04 — Variables & Naming

## Simple Meaning

Variable ek **name** hota hai jisme hum value store karte hain.

```python
name = "Ayan"
age = 21
```

Yaha:

- `name` variable hai
- `"Ayan"` value hai
- `age` variable hai
- `21` value hai

---

## Variable Banane Ka Syntax

```python
variable_name = value
```

Example:

```python
city = "Mumbai"
salary = 50000
is_active = True
```

---

## Python Me Type Declare Nahi Karna Padta

```python
score = 95
```

Python automatically samajh leta hai ki `score` integer hai.

```python
score = "ninety five"
```

Ab same variable string value hold kar raha hai.

Isko **dynamic typing** kehte hain.

---

## Good Variable Names

Good:

```python
employee_name = "Ayan"
monthly_salary = 50000
is_logged_in = True
```

Bad:

```python
x = "Ayan"
a = 50000
b = True
```

Short names kabhi-kabhi loops me okay hote hain, but business logic me meaningful names better hain.

---

## Naming Rules

Allowed:

```python
name = "Ayan"
user_name = "Ayan"
age2 = 21
_private_value = 10
```

Not allowed:

```python
2age = 21
user-name = "Ayan"
user name = "Ayan"
```

Variable name:

- letter ya underscore se start hona chahiye
- number se start nahi ho sakta
- spaces nahi honi chahiye
- special characters generally allowed nahi hote except `_`
- Python keyword use nahi kar sakte

---

## Python Keywords

Examples:

```text
if
else
for
while
class
def
return
True
False
None
```

Inko variable name ke roop me use nahi karna.

Wrong:

```python
class = "A"
```

---

## Snake Case

Python me common naming style:

```python
employee_name = "Ayan"
total_salary = 50000
user_is_active = True
```

Is style ko **snake_case** bolte hain.

---

## Multiple Assignment

```python
name, age, city = "Ayan", 21, "Mumbai"
```

Same value multiple variables ko:

```python
x = y = z = 0
```

---

## Swap Values

Python me easy swap:

```python
a = 10
b = 20

a, b = b, a

print(a)
print(b)
```

Output:

```text
20
10
```

---

## Constants

Python me true constant keyword nahi hai, but convention ke liye uppercase names use karte hain:

```python
MAX_RETRIES = 3
API_TIMEOUT = 30
```

Team ko signal milta hai ki value normally change nahi karni chahiye.

---

## Company Use Case

Suppose employee API ka data process kar rahe ho:

```python
employee_id = 101
employee_name = "Ayan"
department = "Cloud"
is_active = True
```

Clear variable names se dusra developer instantly samajh sakta hai data kya represent karta hai.

---

## Common Mistakes

### Undefined Variable

```python
print(username)
```

Agar `username` pehle define nahi hua to:

```text
NameError
```

### Case Difference

```python
name = "Ayan"
print(Name)
```

`name` aur `Name` same nahi hain.

### Built-in Name Overwrite Karna

Avoid:

```python
list = [1, 2, 3]
str = "hello"
```

Better:

```python
numbers = [1, 2, 3]
message = "hello"
```

Kyunki `list` aur `str` Python ke built-in names hain.

---

## Interview Questions

**Q1. Python dynamically typed language hai?**  
Yes. Variable ka type runtime par value se decide hota hai.

**Q2. Variable naming convention kya hai?**  
Python me variables/functions ke liye commonly `snake_case` use hota hai.

**Q3. Constant kaise represent karte hain?**  
Conventionally uppercase names, jaise `MAX_RETRIES = 3`.

---

## Practice

1. Apna `name`, `age`, `city` variables me store karo.
2. `first_name` aur `last_name` banao.
3. `MAX_LOGIN_ATTEMPTS = 5` constant banao.
4. Do variables ki values swap karo.
5. Intentionally `Name` vs `name` error run karke dekho.

---

## Quick Revision

```text
Variable = named value
Assignment = =
Naming style = snake_case
Python type declaration = not required
Constants convention = UPPER_CASE
Python = case-sensitive
```

⬅️ Previous: [03 — Syntax, Comments & Indentation](03-Syntax-Comments-Indentation.md)  
➡️ Next: [05 — Data Types](05-Data-Types.md)
