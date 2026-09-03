# 07 — Python Operators

## Simple Meaning

Operators symbols/keywords hote hain jo values par operation perform karte hain.

Example:

```python
x = 10
y = 5

print(x + y)
```

Output:

```text
15
```

Yaha `+` operator hai.

---

# 1. Arithmetic Operators

| Operator | Meaning | Example |
|---|---|---|
| `+` | Addition | `10 + 5` |
| `-` | Subtraction | `10 - 5` |
| `*` | Multiplication | `10 * 5` |
| `/` | Division | `10 / 5` |
| `//` | Floor division | `11 // 2` |
| `%` | Remainder | `11 % 2` |
| `**` | Power | `2 ** 3` |

Example:

```python
a = 11
b = 2

print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

Output:

```text
5.5
5
1
121
```

---

# 2. Assignment Operators

```python
x = 10
```

`=` value assign karta hai.

Shortcut:

```python
x = 10
x += 5
print(x)
```

Output:

```text
15
```

Common:

```text
+=
-=
*=
/=
//=
%=
**=
```

---

# 3. Comparison Operators

Comparison ka result boolean hota hai: `True` ya `False`.

| Operator | Meaning |
|---|---|
| `==` | Equal |
| `!=` | Not equal |
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater than or equal |
| `<=` | Less than or equal |

Example:

```python
age = 21

print(age >= 18)
print(age == 20)
```

Output:

```text
True
False
```

---

## `=` vs `==`

Bahut important:

```python
age = 21
```

`=` assignment hai.

```python
age == 21
```

`==` comparison hai.

---

# 4. Logical Operators

## `and`

Dono conditions true honi chahiye.

```python
age = 21
has_id = True

print(age >= 18 and has_id)
```

Output:

```text
True
```

## `or`

At least ek condition true ho.

```python
is_admin = False
is_manager = True

print(is_admin or is_manager)
```

Output:

```text
True
```

## `not`

Boolean ko reverse karta hai.

```python
is_blocked = False
print(not is_blocked)
```

Output:

```text
True
```

---

# 5. Membership Operators

## `in`

```python
skills = ["Python", "AWS", "SQL"]

print("Python" in skills)
```

Output:

```text
True
```

## `not in`

```python
print("Java" not in skills)
```

Output:

```text
True
```

---

# 6. Identity Operators

```text
is
is not
```

Ye check karte hain ki do references **same object** ko point kar rahe hain ya nahi.

```python
a = None

print(a is None)
```

Output:

```text
True
```

`None` check ke liye professional Python code me:

```python
if result is None:
    ...
```

preferred hota hai.

---

## `==` vs `is`

- `==` → values equal hain?
- `is` → same object hai?

Example:

```python
a = [1, 2]
b = [1, 2]

print(a == b)
print(a is b)
```

Usually output:

```text
True
False
```

Values same hain, objects alag hain.

---

# Operator Precedence

```python
result = 2 + 3 * 4
print(result)
```

Output:

```text
14
```

Multiplication pehle hota hai.

Parentheses se intent clear karo:

```python
result = (2 + 3) * 4
```

Output:

```text
20
```

Professional code me complex expressions me parentheses readability improve karte hain.

---

## Company Use Case

Suppose API request process karne se pehle access check karna hai:

```python
is_active = True
role = "admin"

can_access = is_active and role in ["admin", "manager"]
print(can_access)
```

Ye permissions/business rules me common pattern hai.

---

## Common Mistakes

### Assignment vs Comparison

Wrong logic:

```text
=  means assign
== means compare
```

Is difference ko strong rakho.

### `/` vs `//`

```python
print(5 / 2)   # 2.5
print(5 // 2)  # 2
```

### `is` for Normal Value Comparison

Avoid:

```python
name is "Ayan"
```

Use:

```python
name == "Ayan"
```

Use `is` mainly identity checks, especially `None`.

---

## Interview Questions

**Q1. `/` aur `//` me difference?**  
`/` normal division karta hai; `//` floor division.

**Q2. `%` ka use?**  
Remainder nikalta hai. Even/odd checks me common hai.

**Q3. `==` aur `is` ka difference?**  
`==` value equality; `is` object identity.

**Q4. `and` aur `or` ka difference?**  
`and` ko sab conditions true chahiye; `or` ko at least ek true.

---

## Practice

1. User ke marks se check karo marks `>= 40` hain ya nahi.
2. Number even/odd `%` se check karo.
3. `age >= 18 and has_id` expression banao.
4. Skills list me `"Python" in skills` check karo.
5. `==` aur `is` ka list example run karo.

---

## Quick Revision

```text
Math = + - * / // % **
Compare = == != > < >= <=
Logic = and or not
Membership = in / not in
Identity = is / is not
Assign = =
Compare equality = ==
```

⬅️ Previous: [06 — Input & Output](06-Input-and-Output.md)  
➡️ Next: [08 — Type Conversion](08-Type-Conversion.md)
