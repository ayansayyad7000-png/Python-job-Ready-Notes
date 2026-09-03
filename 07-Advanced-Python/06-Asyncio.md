# 06 — Async Python with asyncio

## Simple Meaning
`asyncio` `async` / `await` syntax se concurrent I/O code likhne ka standard-library framework hai.

```python
import asyncio

async def main():
    print("start")
    await asyncio.sleep(1)
    print("done")

asyncio.run(main())
```

## Coroutine
`async def` function call coroutine object return karta hai; use await/run karna hota hai.

## Concurrent Tasks
```python
import asyncio

async def fetch(name, delay):
    await asyncio.sleep(delay)
    return name

async def main():
    results = await asyncio.gather(
        fetch("api-1", 1),
        fetch("api-2", 1),
    )
    print(results)

asyncio.run(main())
```

## Best Fit
Network I/O, many connections, async APIs, non-blocking workflows.

CPU-heavy calculation ke liye async alone magic speed-up nahi deta.

## Interview
- `async def` coroutine function.
- `await` async operation complete hone tak cooperative pause.
- event loop tasks schedule karta hai.
