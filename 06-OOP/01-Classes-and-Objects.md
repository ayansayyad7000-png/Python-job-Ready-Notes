# Classes and Objects

A class defines a type. An object is an instance of that class.

```python
class Server:
    pass

server = Server()
```

## Why OOP Exists
OOP groups data and behavior that belong together.

Example concept:
```text
Server
├── name
├── region
├── status
└── restart()
```

## Company Use
Domain models, service clients, SDK wrappers, configuration objects, reusable components.

## Common Mistakes
- Using classes for tiny problems that simple functions solve better
- Creating "god classes" with too many responsibilities

## Interview Questions
1. Class vs object?
2. When is OOP useful?

## Practice
Create a `User` class and instantiate two users.