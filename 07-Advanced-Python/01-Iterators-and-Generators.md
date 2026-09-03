# Iterators and Generators

## Iterator
An iterator produces values one at a time.

```python
values = iter([10, 20, 30])
print(next(values))
```

Objects used in `for` loops follow the iterator protocol.

## Generator
A generator uses `yield` to produce values lazily.

```python
def read_batches(items, size):
    for i in range(0, len(items), size):
        yield items[i:i + size]
```

## Why Generators Matter
They avoid loading every result into memory at once.

## Company Use
Large files, database batches, streaming data, paginated APIs, ETL pipelines.

## Common Mistakes
- Expecting a generator to be reusable after it is exhausted
- Converting a huge generator to `list()` unnecessarily

## Interview Questions
1. `return` vs `yield`?
2. Iterable vs iterator?

## Practice
Write a generator that yields log lines containing `ERROR`.