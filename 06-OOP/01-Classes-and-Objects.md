# 01 — Classes & Objects

## Simple Meaning
Class blueprint hai; object us blueprint ka instance.

```python
class Server:
    pass

server1 = Server()
```

## Real Example
```python
class Employee:
    def greet(self):
        print("Hello from employee")

employee = Employee()
employee.greet()
```

`self` current object ko represent karta hai.

## Why OOP?
Related data + behavior ko ek structure me organize karta hai.

## Company Use
Users, orders, cloud resources, API clients, services, models ko classes se model kiya ja sakta hai.

## Interview
- class = blueprint.
- object = class instance.
- `self` current instance.

## Practice
1. `Car` class.
2. `Server` class.
3. Method add karo.
