# 03 — break, continue, pass

## `break`
Loop ko immediately stop karta hai.

```python
for number in range(1, 10):
    if number == 5:
        break
    print(number)
```

Output: `1 2 3 4`.

## `continue`
Current iteration skip karta hai, loop continue hota hai.

```python
for number in range(1, 6):
    if number == 3:
        continue
    print(number)
```

Output me `3` skip hoga.

## `pass`
Placeholder hai—kuch nahi karta.

```python
def future_feature():
    pass
```

## Company Example
Invalid records skip:

```python
records = [10, None, 30]

total = 0
for value in records:
    if value is None:
        continue
    total += value

print(total)
```

Search milte hi stop:

```python
users = ["rahul", "ayan", "sameer"]

for user in users:
    if user == "ayan":
        print("Found")
        break
```

## Interview
- `break` → loop stop.
- `continue` → current iteration skip.
- `pass` → no-op placeholder.

## Practice
1. 1–20 me 10 par break.
2. Odd numbers skip karo.
3. Empty function with `pass`.
4. List me first negative number find karke stop.
