# Inheritance and Polymorphism

## Inheritance
A child class can reuse behavior from a parent class.

```python
class Service:
    def start(self):
        print("Starting service")

class APIService(Service):
    pass
```

## Polymorphism
Different objects can provide the same interface with different behavior.

```python
class LocalStorage:
    def save(self, data):
        print("Saved locally")

class S3Storage:
    def save(self, data):
        print("Saved to S3")
```

Code can call `.save()` without caring about the implementation.

## Company Use
Adapters, plugins, storage backends, payment providers, deployment targets.

## Common Mistakes
- Deep inheritance trees
- Using inheritance only to share a few lines of code

## Interview Question
Inheritance vs composition?