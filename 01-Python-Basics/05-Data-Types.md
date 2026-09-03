# 05 — Python Data Types

## Simple Meaning

Data type batata hai variable ke andar **kis type ka data** stored hai.

Example:

```python
name = "Ayan"
age = 21
height = 5.9
is_student = True
```

Yaha:

- `name` → string (`str`)
- `age` → integer (`int`)
- `height` → float (`float`)
- `is_student` → boolean (`bool`)

---

## Important Built-in Data Types

| Type | Meaning | Example |
|---|---|---|
| `str` | Text | `"Ayan"` |
| `int` | Whole number | `21` |
| `float` | Decimal number | `5.9` |
| `bool` | True/False | `True` |
| `list` | Ordered, changeable collection | `[10, 20]` |
| `tuple` | Ordered, fixed collection | `(10, 20)` |
| `set` | Unique values | `{10, 20}` |
| `dict` | Key-value data | `{"name": "Ayan"}` |
| `NoneType` | No value | `None` |

---

## Check Type Using `type()`

```python
name = "Ayan"
age = 21

print(type(name))
print(type(age))
```

Output:

```text
<class 'str'>
<class 'int'>
```

---

# 1. String — `str`

Text data.

```python
name = "Ayan"
role = 'AI Platform Engineer'
```

Single aur double quotes dono valid hain.

```python
message = "Python is easy"
print(message)
```

---

# 2. Integer — `int`

Whole numbers:

```python
age = 21
employees = 100
balance = -500
```

---

# 3. Float — `float`

Decimal values:

```python
price = 99.99
cpu_usage = 67.5
```

---

# 4. Boolean — `bool`

Sirf two values:

```python
True
False
```

Example:

```python
is_logged_in = True
server_down = False
```

Boolean values conditions me bahut use hote hain.

---

# 5. List

Multiple values store kar sakti hai aur change ho sakti hai.

```python
skills = ["Python", "AWS", "Linux"]
```

Index:

```python
print(skills[0])
```

Output:

```text
Python
```

List ko later detail me cover karenge.

---

# 6. Tuple

List jaisa ordered collection, but normally immutable hota hai.

```python
coordinates = (19.07, 72.87)
```

---

# 7. Set

Unique values store karta hai.

```python
services = {"EC2", "S3", "EC2"}
print(services)
```

Duplicate `EC2` repeat nahi hota.

---

# 8. Dictionary — `dict`

Key-value format.

```python
employee = {
    "name": "Ayan",
    "role": "AI Platform Engineer",
    "experience": 0
}
```

Value access:

```python
print(employee["role"])
```

---

# 9. None

`None` ka meaning: currently koi value nahi.

```python
result = None
```

Ye empty string `""` ya zero `0` se different hai.

---

## Mutable vs Immutable — First Idea

### Mutable
Change ho sakta hai:

```text
list
dict
set
```

### Immutable
Existing object directly change nahi hota:

```text
int
float
bool
str
tuple
```

Ye concept later bahut important hoga functions aur memory behavior me.

---

## Company Example

API se employee data aa sakta hai:

```python
employee = {
    "id": 101,
    "name": "Ayan",
    "skills": ["Python", "AWS", "SQL"],
    "salary": 55000.50,
    "active": True,
    "manager": None
}
```

Ek hi object me different data types use hue.

---

## Common Mistakes

### Number ko String Samajhna

```python
age = "21"
```

Ye integer nahi, string hai.

Check:

```python
print(type(age))
```

### Boolean Quotes Me

```python
is_active = "False"
```

Ye string hai aur non-empty string truthy hoti hai.

Actual boolean:

```python
is_active = False
```

---

## Interview Questions

**Q1. Python ke common built-in data types kaunse hain?**  
`str`, `int`, `float`, `bool`, `list`, `tuple`, `set`, `dict`, `NoneType`.

**Q2. List aur tuple ka basic difference?**  
List mutable hoti hai; tuple immutable hota hai.

**Q3. `None` kya represent karta hai?**  
Absence of a value / no value.

**Q4. Variable ka type kaise check karte hain?**  
`type(variable)`.

---

## Practice

1. Har basic data type ka ek variable banao.
2. Sab par `type()` run karo.
3. Ek employee dictionary banao.
4. Skills ki list banao.
5. `"100"` aur `100` ka type compare karo.

---

## Quick Revision

```text
Text = str
Whole number = int
Decimal = float
True/False = bool
Collection = list / tuple / set
Key-value = dict
No value = None
Check type = type()
```

⬅️ Previous: [04 — Variables & Naming](04-Variables-and-Naming.md)  
➡️ Next: [06 — Input & Output](06-Input-and-Output.md)
