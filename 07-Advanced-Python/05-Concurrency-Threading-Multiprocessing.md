# Threading and Multiprocessing

## Threading
Useful mainly for I/O-bound work such as waiting on files, APIs, or networks.

```python
from concurrent.futures import ThreadPoolExecutor

def fetch(item):
    return item

with ThreadPoolExecutor(max_workers=4) as pool:
    results = list(pool.map(fetch, range(10)))
```

## Multiprocessing
Useful for CPU-heavy work because separate processes can run Python code independently.

```python
from concurrent.futures import ProcessPoolExecutor
```

## Company Use
Parallel API calls, file processing, CPU-heavy transformations, worker jobs.

## Key Idea
Choose based on workload, not because parallelism looks faster.

## Common Mistakes
- Sharing mutable state across threads without care
- Creating too many workers
- Using multiprocessing for tiny tasks where overhead dominates

## Interview Question
When would you choose threads vs processes?