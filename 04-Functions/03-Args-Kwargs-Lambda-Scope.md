# *args, **kwargs, Lambda and Scope

## *args
Collects extra positional arguments.
```python
def total(*values):
    return sum(values)
```

## **kwargs
Collects extra keyword arguments.
```python
def show_config(**config):
    return config
```

## Lambda
Small anonymous function.
```python
square = lambda x: x * x
```
Use lambdas for short expressions, not complex business logic.

## Scope
Variables can be local, enclosing, global, or built-in.

```python
x = 10

def demo():
    x = 20
    print(x)
```

## Company Use
Flexible utility functions, callbacks, sorting keys, adapters.

## Common Mistakes
- Overusing `*args`/`**kwargs` and hiding required inputs
- Using global variables for shared mutable state

## Interview Questions
1. What does `*args` collect?
2. What does `**kwargs` collect?
3. What is local scope?

## Practice
Create a logging helper that accepts a message plus optional metadata using `**kwargs`.