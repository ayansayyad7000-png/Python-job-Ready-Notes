# Constructor, Attributes and Methods

`__init__` initializes a new object.

```python
class Server:
    def __init__(self, name, region):
        self.name = name
        self.region = region
        self.status = "stopped"

    def start(self):
        self.status = "running"

server = Server("api-1", "ap-south-1")
server.start()
```

## self
`self` refers to the current instance.

## Instance Attributes
`self.name` and `self.status` can differ between objects.

## Company Use
Objects can hold state and expose safe operations on that state.

## Common Mistakes
- Forgetting `self`
- Putting unrelated behavior in one class

## Interview Questions
1. What does `__init__` do?
2. What is `self`?

## Practice
Build an `Employee` class with a method that calculates annual salary.