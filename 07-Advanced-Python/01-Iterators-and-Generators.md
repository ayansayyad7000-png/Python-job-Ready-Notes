# 01 — Iterators & Generators

## Iterator
Iterator ek object hai jisse values one-by-one milti hain.

```python
numbers = iter([10, 20, 30])
print(next(numbers))
print(next(numbers))
```

`for` loop internally iteration protocol use karta hai.

## Generator
Generator lazy values produce karta hai using `yield`.

```python
def count_up_to(limit):
    n = 1
    while n <= limit:
        yield n
        n += 1

for n in count_up_to(3):
    print(n)
```

## Why Useful?
Large data ko memory me ek saath load karne ki zarurat nahi.

```python
def read_large_file(path):
    with open(path, encoding="utf-8") as file:
        for line in file:
            yield line.strip()
```

## Generator Expression
```python
squares = (n * n for n in range(1_000_000))
```

## Company Use
Large logs, CSV rows, streaming records, pipelines.

## Interview
- iterable can produce iterator.
- iterator supports `next()`.
- generator uses `yield` and lazy evaluation.
- list usually eager; generator memory-efficient.
