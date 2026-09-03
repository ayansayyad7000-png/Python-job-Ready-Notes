# Loops: for and while

## for Loop
Use when iterating over a collection or known sequence.

```python
servers = ["api-1", "api-2", "worker-1"]
for server in servers:
    print(server)
```

## range()
```python
for i in range(1, 6):
    print(i)
```

## while Loop
Use while a condition remains true.

```python
retries = 3
while retries > 0:
    print("Trying...")
    retries -= 1
```

## Company Use
Processing records, polling, retries, batch jobs, file scanning.

## Common Mistakes
- Infinite `while` loops
- Modifying a collection incorrectly while iterating

## Interview Questions
1. `for` vs `while`?
2. What does `range(5)` generate?

## Practice
Loop through a list of CPU values and print only values above 80.