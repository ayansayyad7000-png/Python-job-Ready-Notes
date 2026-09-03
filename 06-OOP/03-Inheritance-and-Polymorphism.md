# 03 — Inheritance & Polymorphism

## Inheritance
Child class parent ka behavior reuse karta hai.

```python
class CloudResource:
    def status(self):
        return "unknown"

class EC2Instance(CloudResource):
    def status(self):
        return "running"
```

## `super()`
```python
class Employee:
    def __init__(self, name):
        self.name = name

class Engineer(Employee):
    def __init__(self, name, skill):
        super().__init__(name)
        self.skill = skill
```

## Polymorphism
Same method interface, different behavior:

```python
resources = [EC2Instance()]
for resource in resources:
    print(resource.status())
```

## Company Note
Inheritance useful hai but overuse se tight coupling ho sakta hai. Composition often cleaner alternative hota hai.

## Interview
- inheritance = reuse/relationship.
- method overriding child behavior customize karta hai.
- polymorphism same interface different implementations.
