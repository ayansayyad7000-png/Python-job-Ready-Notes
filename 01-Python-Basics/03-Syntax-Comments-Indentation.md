# 03 — Syntax, Comments & Indentation

## Simple Meaning

**Syntax** matlab Python code likhne ke rules.

Jaise English me grammar hoti hai, waise programming language me syntax hota hai.

---

## Basic Python Syntax

```python
name = "Ayan"
print(name)
```

Output:

```text
Ayan
```

Python me semicolon `;` normally required nahi hota.

---

## Python is Case-Sensitive

```python
name = "Ayan"
Name = "Rahul"

print(name)
print(Name)
```

Output:

```text
Ayan
Rahul
```

`name` aur `Name` alag variables hain.

---

# Comments

Comments code explain karne ke liye use hote hain. Python comments execute nahi karta.

## Single-Line Comment

```python
# This is a comment
print("Hello")
```

## Inline Comment

```python
age = 21  # user age
```

Good comments **why** explain karte hain, obvious code repeat nahi karte.

Bad:

```python
age = 21  # set age to 21
```

Better:

```python
age = 21  # minimum age used for this test account
```

---

# Indentation

Python me indentation bahut important hai.

Example:

```python
age = 20

if age >= 18:
    print("Eligible")
```

`print()` ke pehle spaces batate hain ki ye line `if` block ke andar hai.

Wrong:

```python
if age >= 18:
print("Eligible")
```

Isse `IndentationError` aayega.

---

## Standard Indentation

Python code me normally **4 spaces** use karte hain.

```python
if True:
    print("Inside block")
```

---

# Code Blocks

Colon `:` ke baad often indented block aata hai.

Examples:

```python
if condition:
    pass
```

```python
for item in items:
    pass
```

```python
def greet():
    pass
```

```python
class User:
    pass
```

`pass` ka meaning: abhi kuch execute nahi karna, but syntactically block empty nahi reh sakta.

---

## Multi-Line Statements

Long code ko readable banane ke liye parentheses use kar sakte ho.

```python
total = (
    100
    + 200
    + 300
)

print(total)
```

Output:

```text
600
```

---

## Company Use

Professional code me readable formatting important hai because code ek hi person nahi, puri team maintain karti hai.

Bad formatting:

```python
if user_active:
 print("active")
```

Clean formatting:

```python
if user_active:
    print("active")
```

Companies often formatters/lint tools use karti hain, jaise:

- Black
- Ruff
- Flake8

Ye later clean-code section me cover honge.

---

## Common Mistakes

### Missing Colon

Wrong:

```python
if age >= 18
    print("Adult")
```

Correct:

```python
if age >= 18:
    print("Adult")
```

### Wrong Indentation

Different indentation levels logic change kar sakte hain.

```python
if logged_in:
    print("Welcome")

print("Program finished")
```

Second print `if` ke bahar hai.

---

## Interview Questions

**Q1. Python indentation kyu important hai?**  
Indentation code blocks define karti hai. Ye sirf styling nahi, Python syntax ka part hai.

**Q2. Python case-sensitive hai?**  
Yes.

**Q3. Comment ka purpose kya hai?**  
Code ka intent/important reasoning explain karna without execution.

---

## Practice

1. `name` aur `Name` variables bana kar difference check karo.
2. Ek `if` block likho with correct 4-space indentation.
3. 3 useful comments likho.
4. Missing colon wala code intentionally run karke error dekho.

---

## Quick Revision

```text
Syntax = code rules
Comments = #
Indentation = code block
Recommended indentation = 4 spaces
Python = case-sensitive
```

⬅️ Previous: [02 — Installation & Setup](02-Installation-and-Setup.md)  
➡️ Next: [04 — Variables & Naming](04-Variables-and-Naming.md)
