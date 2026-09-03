# 03 — *args, **kwargs, Lambda & Scope

## `*args`
Variable positional arguments:

```python
def total(*numbers):
    return sum(numbers)

print(total(10, 20, 30))
```

Inside function `numbers` tuple hota hai.

## `**kwargs`
Variable keyword arguments:

```python
def show_config(**config):
    for key, value in config.items():
        print(key, value)

show_config(region="ap-south-1", debug=True)
```

Inside function `config` dict hota hai.

## Lambda
Small anonymous function:

```python
square = lambda x: x * x
print(square(5))
```

Common sorting example:
```python
users = [{"name": "A", "age": 30}, {"name": "B", "age": 20}]
users.sort(key=lambda user: user["age"])
```

## Scope
```python
name = "Global"

def demo():
    name = "Local"
    print(name)
```

Local variable function ke andar limited hota hai.

Avoid unnecessary `global`; values parameters/return se pass karna cleaner hota hai.

## Interview
- `*args` → tuple of positional args.
- `**kwargs` → dict of keyword args.
- lambda → small anonymous function.
- Local vs global scope.

## Practice
1. `*args` average.
2. `**kwargs` employee profile.
3. Sort dict list by salary using lambda.
4. Scope example run karo.
