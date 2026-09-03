# break, continue and pass

## break
Stops the loop.
```python
for n in range(10):
    if n == 5:
        break
```

## continue
Skips the current iteration.
```python
for n in range(5):
    if n == 2:
        continue
    print(n)
```

## pass
A placeholder that does nothing.
```python
def future_feature():
    pass
```

## Company Use
- `break`: stop searching after a match
- `continue`: skip invalid records
- `pass`: temporary placeholder during development

## Common Mistake
Using `pass` when `continue` or `break` was intended.

## Practice
Loop over records, skip inactive users, and stop after finding an administrator.