# 05 — Threading & Multiprocessing

## Why Concurrency?
Ek program multiple tasks ko efficiently handle kar sake.

## Threading
I/O-bound tasks (network/file waiting) ke liye useful.

```python
from concurrent.futures import ThreadPoolExecutor


def check(url):
    return f"checked {url}"

urls = ["a", "b", "c"]
with ThreadPoolExecutor(max_workers=3) as pool:
    results = list(pool.map(check, urls))
```

## Multiprocessing
CPU-heavy work ko separate processes me run kar sakta hai.

```python
from concurrent.futures import ProcessPoolExecutor


def square(n):
    return n * n

if __name__ == "__main__":
    with ProcessPoolExecutor() as pool:
        print(list(pool.map(square, range(5))))
```

## Important Thinking
- I/O-bound → threads/async often useful.
- CPU-bound → process pool often useful.
- Shared state/race conditions se careful.

## Company Use
Parallel API calls, batch jobs, CPU transforms.

## Interview
Concurrency = overlapping tasks. Parallelism = tasks literally same time multiple cores/resources par execute ho sakte hain.
