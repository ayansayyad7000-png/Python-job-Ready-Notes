# 09 — Level 1 Practice: Python Basics

## How to Use This File

Har question pehle khud solve karo. Direct solution mat dekho.

Recommended flow:

```text
Read problem
   ↓
Write code yourself
   ↓
Run it
   ↓
Test different inputs
   ↓
Fix errors
   ↓
Then compare with solution idea
```

---

# Part A — Very Basic

## Q1. Hello Developer

Output exactly ye print karo:

```text
Hello Ayan
I am learning Python for real company work.
```

Concepts: `print()`

---

## Q2. Personal Profile

Variables banao:

```text
name
age
city
role
```

f-string use karke ek sentence print karo.

Example output:

```text
My name is Ayan, I am 21 years old, I live in Mumbai and I am learning AI Platform Engineering.
```

Concepts: variables, strings, f-strings

---

## Q3. Type Checker

Ye variables banao:

```python
name = "Ayan"
age = 21
salary = 45000.50
is_active = True
```

Har variable ka `type()` print karo.

Concepts: data types, `type()`

---

# Part B — Input & Conversion

## Q4. Age Calculator

User se birth year aur current year input lo. Approximate age calculate karo.

Example:

```text
Birth year: 2005
Current year: 2026
Age: 21
```

Concepts: `input()`, `int()`, subtraction

---

## Q5. Salary Calculator

User se monthly salary input lo aur annual salary calculate karo.

Example:

```text
Monthly salary: 50000
Annual salary: 600000.00
```

Concepts: `float()`, multiplication, f-string formatting

---

## Q6. Bill Calculator

Inputs:

```text
product_name
price
quantity
```

Output:

```text
Product: Keyboard
Price: 1500.00
Quantity: 2
Total: 3000.00
```

Concepts: strings, float, int, multiplication

---

# Part C — Operators

## Q7. Even or Odd Expression

Ek number store karo aur `%` operator use karke remainder print karo.

Example:

```python
number = 10
```

Expected remainder:

```text
0
```

Next level me condition laga kar `Even` / `Odd` print karenge.

---

## Q8. Access Check Expression

Variables:

```python
age = 21
has_id = True
```

Expression banao jo check kare:

```text
age >= 18 AND has_id is True
```

Output should be boolean.

---

## Q9. Skill Membership

```python
skills = ["Python", "AWS", "Linux", "SQL"]
```

Check karo:

```text
Python list me hai?
Java list me nahi hai?
```

Use `in` and `not in`.

---

# Part D — Company-Style Thinking

## Q10. Employee Record

Ek dictionary banao:

```text
id
name
role
skills
salary
active
manager
```

Suggested data types carefully choose karo.

Example idea:

```python
employee = {
    "id": 101,
    "name": "Ayan",
    "role": "AI Platform Engineer",
    "skills": ["Python", "AWS", "SQL"],
    "salary": 55000.0,
    "active": True,
    "manager": None,
}
```

Then `name`, `role` and first skill print karo.

---

## Q11. Server Configuration

Variables banao:

```text
SERVER_NAME
port
cpu_usage
is_healthy
```

Good naming conventions use karo. `SERVER_NAME` ko constant-style name rakho.

---

## Q12. Environment Input

User se environment input lo:

```text
dev
staging
prod
```

Input ko clean karo using:

```python
.strip().lower()
```

Example:

```python
environment = input("Environment: ").strip().lower()
```

Print selected environment.

Concepts: input, strings, clean data

---

# Part E — Predict the Output

Code run karne se pehle output guess karo.

## Q13

```python
x = "10"
y = "20"
print(x + y)
```

## Q14

```python
x = 10
y = 3
print(x // y)
print(x % y)
```

## Q15

```python
print(bool(0))
print(bool("0"))
print(bool(""))
```

## Q16

```python
a = [1, 2]
b = [1, 2]
print(a == b)
print(a is b)
```

---

# Mini Project — Employee Salary Summary

Build a small CLI program.

### Input

- employee name
- employee ID
- monthly salary
- bonus percentage

### Calculate

```text
annual_salary = monthly_salary * 12
bonus_amount = annual_salary * bonus_percentage / 100
final_compensation = annual_salary + bonus_amount
```

### Example Output

```text
========== EMPLOYEE SUMMARY ==========
Employee ID: 101
Name: Ayan
Monthly Salary: 50000.00
Annual Salary: 600000.00
Bonus: 60000.00
Final Compensation: 660000.00
======================================
```

### Skills Used

- variables
- naming
- `input()`
- `int()` / `float()`
- arithmetic operators
- f-strings
- formatted output

---

# Self-Check

Level 2 par jane se pehle tumhe ye bina notes dekhe aana chahiye:

- [ ] Python file run karna
- [ ] variables banana
- [ ] good variable names likhna
- [ ] common data types identify karna
- [ ] `type()` use karna
- [ ] `input()` use karna
- [ ] string input ko number me convert karna
- [ ] f-string use karna
- [ ] arithmetic operators use karna
- [ ] comparison operators samajhna
- [ ] `and`, `or`, `not` ka basic idea
- [ ] `in` / `not in` use karna
- [ ] `==` aur `is` ka basic difference

---

## Interview Rapid Fire

1. Python case-sensitive hai?
2. `input()` kya return karta hai?
3. `=` aur `==` me difference?
4. `/` aur `//` me difference?
5. `%` kya karta hai?
6. `bool("False")` ka result kya hai?
7. `None` ka meaning kya hai?
8. list aur tuple ka basic difference?
9. `type()` ka use?
10. `is` aur `==` me difference?

Agar in 10 ka answer confidently de sakte ho, tumhari basic foundation strong ho rahi hai.

---

⬅️ Previous: [08 — Type Conversion](08-Type-Conversion.md)  
➡️ Next Level: **Conditions & Logic Building**
