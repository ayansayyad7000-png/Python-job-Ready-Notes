# 02 — Constructor, Attributes & Methods

## `__init__`
Object creation ke time initialize:

```python
class Employee:
    def __init__(self, name, role):
        self.name = name
        self.role = role

    def describe(self):
        return f"{self.name} - {self.role}"

employee = Employee("Ayan", "Platform")
print(employee.describe())
```

## Instance Attributes
`self.name`, `self.role` har object ki values ho sakti hain.

## Class Attribute
```python
class Employee:
    company = "ExampleCorp"
```

Shared class-level data.

## Method Types First Look
- instance method → `self`
- class method → `cls`
- static method → neither instance nor class state required

```python
class Math:
    @staticmethod
    def add(a, b):
        return a + b
```

## Interview
`__init__` initializer method hai, object state setup karta hai.
