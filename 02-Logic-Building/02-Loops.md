# 02 — Loops: for and while

## Simple Meaning
Loop same work repeat karta hai without duplicate code.

# `for` Loop
Collection/range ke items par iterate karne ke liye:

```python
skills = ["Python", "AWS", "SQL"]

for skill in skills:
    print(skill)
```

## `range()`
```python
for number in range(1, 6):
    print(number)
```

Output: `1` to `5`. Stop value include nahi hoti.

```python
range(start, stop, step)
```

Example:
```python
for n in range(0, 10, 2):
    print(n)
```

# `while` Loop
Jab tak condition true hai tab tak repeat:

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

## Infinite Loop Warning
```python
count = 1
while count <= 5:
    print(count)
```

`count` update nahi hua, so loop infinite ho sakta hai.

## Company Example
```python
servers = ["api-1", "api-2", "worker-1"]

for server in servers:
    print(f"Checking {server}")
```

Automation, data processing aur API responses me loops common hain.

## `enumerate()` First Look
```python
skills = ["Python", "AWS", "SQL"]

for index, skill in enumerate(skills, start=1):
    print(index, skill)
```

## Interview
**Q. `for` vs `while`?**  
`for` known collection/range iteration ke liye; `while` condition-based repetition ke liye.

**Q. `range(5)` values?**  
`0,1,2,3,4`.

## Practice
1. 1–10 print.
2. Even numbers 2–20.
3. Skills list print.
4. 5 ka table.
5. `while` se countdown 5 to 1.
