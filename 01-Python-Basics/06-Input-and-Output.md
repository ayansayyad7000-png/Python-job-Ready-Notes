# 06 — Input & Output

## Simple Meaning

Program ko user se data lena ho to `input()` use karte hain.

Program ko result dikhana ho to `print()` use karte hain.

---

# Output Using `print()`

```python
print("Hello")
```

Output:

```text
Hello
```

Multiple values:

```python
name = "Ayan"
age = 21

print(name, age)
```

Output:

```text
Ayan 21
```

---

## `sep` Parameter

```python
print("Python", "AWS", "Linux", sep=" | ")
```

Output:

```text
Python | AWS | Linux
```

---

## `end` Parameter

Normally `print()` ke baad new line aati hai.

```python
print("Hello", end=" ")
print("Ayan")
```

Output:

```text
Hello Ayan
```

---

# Input Using `input()`

```python
name = input("Enter your name: ")
print(name)
```

Example:

```text
Enter your name: Ayan
Ayan
```

---

## Important: `input()` Returns String

```python
age = input("Enter age: ")
print(type(age))
```

Agar user `21` enter kare, tab bhi type:

```text
<class 'str'>
```

Number chahiye to convert karo:

```python
age = int(input("Enter age: "))
```

---

# f-Strings

Modern Python me variables ko text ke saath display karne ka clean way:

```python
name = "Ayan"
age = 21

print(f"My name is {name} and I am {age} years old.")
```

Output:

```text
My name is Ayan and I am 21 years old.
```

---

## Expressions Inside f-Strings

```python
price = 100
quantity = 3

print(f"Total = {price * quantity}")
```

Output:

```text
Total = 300
```

---

## Decimal Formatting

```python
price = 99.9876
print(f"Price: {price:.2f}")
```

Output:

```text
Price: 99.99
```

`.2f` means 2 decimal places.

---

# Mini Program

```python
name = input("Enter employee name: ")
salary = float(input("Enter monthly salary: "))

print(f"Employee: {name}")
print(f"Monthly Salary: ₹{salary:.2f}")
print(f"Annual Salary: ₹{salary * 12:.2f}")
```

### What Happens

1. User ka naam input hota hai.
2. Salary input string ke form me aati hai.
3. `float()` salary ko number banata hai.
4. Annual salary calculate hoti hai.
5. f-string clean output dikhata hai.

---

## Company Use Case

CLI tools aur automation scripts me user/environment se input mil sakta hai.

Example:

```python
environment = input("Environment (dev/prod): ").strip().lower()
print(f"Selected environment: {environment}")
```

Real production tools me input ko blindly trust nahi karte; validate karte hain. Validation later cover hoga.

---

## Common Mistakes

### Adding Input Without Conversion

```python
a = input("A: ")
b = input("B: ")

print(a + b)
```

If input is `10` and `20`, output:

```text
1020
```

Because both are strings.

Correct:

```python
a = int(input("A: "))
b = int(input("B: "))

print(a + b)
```

Output:

```text
30
```

### Old String Concatenation

Works:

```python
print("Hello " + name)
```

But f-string usually cleaner:

```python
print(f"Hello {name}")
```

---

## Interview Questions

**Q1. `input()` ka return type kya hota hai?**  
String (`str`).

**Q2. f-string kya hai?**  
String formatting ka readable method jisme `{}` ke andar variables/expressions insert karte hain.

**Q3. `print()` me `sep` aur `end` ka use?**  
`sep` multiple values ke beech separator control karta hai; `end` print ke end me kya aaye wo control karta hai.

---

## Practice

1. Name aur city input lekar sentence print karo.
2. 2 numbers input lekar sum print karo.
3. Product price aur quantity lekar total calculate karo.
4. Temperature input lekar f-string me 1 decimal place show karo.
5. Employee monthly salary se annual salary calculate karo.

---

## Quick Revision

```text
Output = print()
Input = input()
input() return = str
Number input = int(input(...)) / float(input(...))
Modern formatting = f"...{value}..."
```

⬅️ Previous: [05 — Data Types](05-Data-Types.md)  
➡️ Next: [07 — Operators](07-Operators.md)
