# 08 — Type Conversion

## Simple Meaning

Type conversion ka matlab ek data type ko dusre data type me convert karna.

Example:

```python
age = "21"
age = int(age)
```

Pehle `age` string tha, baad me integer ban gaya.

---

## Common Conversion Functions

| Function | Converts To |
|---|---|
| `int()` | Integer |
| `float()` | Float |
| `str()` | String |
| `bool()` | Boolean |
| `list()` | List |
| `tuple()` | Tuple |
| `set()` | Set |

---

# String to Integer

```python
value = "100"
number = int(value)

print(number)
print(type(number))
```

Output:

```text
100
<class 'int'>
```

---

# Integer to String

```python
employee_id = 101
message = "Employee ID: " + str(employee_id)

print(message)
```

Output:

```text
Employee ID: 101
```

f-string usually cleaner hai:

```python
print(f"Employee ID: {employee_id}")
```

---

# Integer to Float

```python
amount = 100
amount = float(amount)

print(amount)
```

Output:

```text
100.0
```

---

# Float to Integer

```python
price = 99.99
whole = int(price)

print(whole)
```

Output:

```text
99
```

Important: `int()` float ko round nahi karta; decimal part remove karta hai.

```python
print(int(9.9))
```

Output:

```text
9
```

---

# Input Conversion

`input()` always string return karta hai.

Wrong for math:

```python
age = input("Enter age: ")
```

Better:

```python
age = int(input("Enter age: "))
```

For decimal:

```python
salary = float(input("Enter salary: "))
```

---

# Conversion Can Fail

```python
value = "Ayan"
number = int(value)
```

Error:

```text
ValueError
```

Kyunki `"Ayan"` valid integer text nahi hai.

Later exception handling me safe conversion karenge:

```python
try:
    number = int(value)
except ValueError:
    print("Invalid number")
```

---

# Boolean Conversion

Python me kuch values falsy hoti hain:

```python
print(bool(0))
print(bool(""))
print(bool([]))
print(bool(None))
```

Output:

```text
False
False
False
False
```

Common truthy values:

```python
print(bool(1))
print(bool("hello"))
print(bool([1, 2]))
```

Output:

```text
True
True
True
```

Important:

```python
print(bool("False"))
```

Output:

```text
True
```

Because `"False"` ek non-empty string hai.

---

# List / Tuple / Set Conversion

```python
numbers = (1, 2, 3)
print(list(numbers))
```

Output:

```text
[1, 2, 3]
```

List to tuple:

```python
values = [10, 20]
print(tuple(values))
```

List to set removes duplicates:

```python
values = [1, 1, 2, 2, 3]
print(set(values))
```

Output contains unique values:

```text
{1, 2, 3}
```

---

## Company Use Case

API, environment variables aur form inputs often strings ke form me milte hain.

Example environment setting:

```python
port_text = "8000"
port = int(port_text)
```

Database/API data process karte waqt correct type bahut important hota hai.

Example:

```python
user_id = int("101")
price = float("499.50")
```

Wrong type business logic ko break kar sakta hai.

---

## Common Mistakes

### Invalid Numeric String

```python
int("10.5")
```

Ye direct integer conversion fail karega.

Possible conversion:

```python
int(float("10.5"))
```

Result:

```text
10
```

But data loss samajhna important hai.

### Assuming `bool("False")` is False

Wrong assumption.

```python
bool("False")
```

is `True` because string empty nahi hai.

---

## Interview Questions

**Q1. `input()` ka output number hota hai?**  
Nahi. `input()` string return karta hai.

**Q2. `int(9.9)` kya return karega?**  
`9`, because decimal part truncate hota hai.

**Q3. `bool("")` kya hai?**  
`False`.

**Q4. `bool("False")` kya hai?**  
`True`, because it is a non-empty string.

**Q5. Invalid string ko `int()` karne par?**  
`ValueError`.

---

## Practice

1. `"250"` ko integer me convert karo.
2. `500` ko string me convert karo.
3. `"89.5"` ko float me convert karo.
4. User se 2 numbers input lekar sum nikalo.
5. `[1, 1, 2, 3, 3]` ko set me convert karke duplicates remove karo.
6. `bool(0)`, `bool(1)`, `bool("")`, `bool("0")` ka output predict karo.

---

## Quick Revision

```text
int()   → integer
float() → decimal
str()   → text
bool()  → True/False
input() → always str
Invalid conversion → ValueError
```

⬅️ Previous: [07 — Operators](07-Operators.md)  
➡️ Next: [Level 1 Practice](09-Level-1-Practice.md)
