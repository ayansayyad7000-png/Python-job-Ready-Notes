# asyncio and async/await

`asyncio` is Python's standard framework for asynchronous I/O.

```python
import asyncio

async def task(name):
    await asyncio.sleep(1)
    return name

async def main():
    results = await asyncio.gather(task("a"), task("b"))
    print(results)

asyncio.run(main())
```

## Key Terms
- `async def`: defines a coroutine
- `await`: waits without blocking the event loop
- `asyncio.gather()`: runs multiple awaitables concurrently

## Company Use
High-concurrency APIs, network clients, event-driven services, many simultaneous I/O operations.

## Common Mistakes
- Calling blocking code inside async functions
- Forgetting `await`
- Using async when simple synchronous code is enough

## Interview Question
Concurrency vs parallelism?

## Practice
Run three async tasks with different delays and collect their results.