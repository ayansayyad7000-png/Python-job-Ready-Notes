# 05 — OOP Project Pattern

## Mini Example: Server Monitor

```python
class Server:
    def __init__(self, name, cpu, memory):
        self.name = name
        self.cpu = cpu
        self.memory = memory

    def health(self):
        if self.cpu >= 90 or self.memory >= 90:
            return "CRITICAL"
        if self.cpu >= 75 or self.memory >= 75:
            return "WARNING"
        return "HEALTHY"

servers = [
    Server("api-1", 45, 60),
    Server("worker-1", 92, 50),
]

for server in servers:
    print(server.name, server.health())
```

## Company Thinking
Class tab useful hai jab data + behavior naturally ek entity ko belong kare.

Avoid class just because OOP padha hai. Simple function better ho to function use karo.

## Practice Project
Build `S3File` class:
- bucket
- key
- size
- `uri()` method
- `is_large()` method

Then multiple objects list me create karo.

## OOP Self Check
- [ ] class/object
- [ ] self
- [ ] __init__
- [ ] instance attribute
- [ ] method
- [ ] inheritance
- [ ] overriding
- [ ] property
- [ ] abstraction idea
