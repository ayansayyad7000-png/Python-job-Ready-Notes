# 01 — What is Python?

## Simple Meaning

Python ek **high-level programming language** hai. Iska syntax simple aur readable hota hai, isliye beginner ke liye easy hai aur companies me automation, backend, data, AI/ML, testing aur cloud work me bahut use hota hai.

Simple words me:

> Python = computer ko instructions dene ka easy aur powerful way.

---

## Your First Python Program

```python
print("Hello, Ayan!")
```

### Output

```text
Hello, Ayan!
```

### Line-by-Line

```python
print("Hello, Ayan!")
```

- `print()` Python ka built-in function hai.
- Iska kaam terminal/screen par output dikhana hai.
- Text ko quotes ke andar likhte hain.

---

## Why Companies Use Python

Python ka use different areas me hota hai:

| Area | Example |
|---|---|
| Backend | APIs, business logic, web services |
| Automation | Files, reports, repetitive tasks |
| Cloud | AWS automation using boto3 |
| DevOps | Deployment/support scripts |
| Data | CSV, Excel, SQL, Pandas |
| AI/ML | Training, inference, data pipelines |
| Testing | Automated tests |

---

## Important Python Features

### 1. Easy to Read

```python
age = 21
if age >= 18:
    print("Adult")
```

Code English jaisa readable lagta hai.

### 2. Dynamically Typed

Variable ka type alag se declare nahi karna padta.

```python
name = "Ayan"
age = 21
```

### 3. Huge Ecosystem

Python ke thousands of libraries/packages available hain, jaise:

- `requests`
- `pandas`
- `numpy`
- `fastapi`
- `pytest`
- `boto3`

### 4. Cross-Platform

Python Windows, Linux aur macOS par run kar sakta hai.

---

## Python File Extension

Python file ka extension:

```text
.py
```

Example:

```text
app.py
main.py
automation.py
```

Run:

```bash
python app.py
```

Ya kuch systems par:

```bash
python3 app.py
```

---

## Interpreter Kya Hota Hai?

Python normally interpreter ke through code execute karta hai.

Simple flow:

```text
Your Python Code
      ↓
Python Interpreter
      ↓
Computer executes instructions
```

---

## Common Beginner Mistakes

### Mistake 1 — `Print` instead of `print`

Wrong:

```python
Print("Hello")
```

Correct:

```python
print("Hello")
```

Python **case-sensitive** hai.

### Mistake 2 — Quotes bhool jana

Wrong:

```python
print(Hello)
```

Correct:

```python
print("Hello")
```

---

## Company Use Case

Suppose company ko daily server health report generate karna hai. Python script automatically:

1. server data read karega,
2. errors check karega,
3. report banayega,
4. team ko result bhej sakta hai.

Ye repetitive manual work automate ho jata hai.

---

## Interview Questions

**Q1. Python kya hai?**  
Python ek high-level, interpreted, general-purpose programming language hai jo readable syntax aur large ecosystem ke liye popular hai.

**Q2. Python case-sensitive hai?**  
Yes. `name`, `Name` aur `NAME` different identifiers hain.

**Q3. Python ka use kaha hota hai?**  
Backend, automation, cloud, data engineering, AI/ML, testing, scripting aur DevOps me.

---

## Practice Tasks

1. `Hello World` print karo.
2. Apna naam print karo.
3. Ek line me `Python Job Ready Journey` print karo.
4. `print()` use karke 3 alag lines output karo.

---

## Quick Revision

```text
Python = simple + powerful programming language
File = .py
Output = print()
Case-sensitive = Yes
Used in = Backend, Cloud, Automation, Data, AI/ML, Testing
```

➡️ Next: [02 — Installation & Setup](02-Installation-and-Setup.md)
