# Arguments and Return Values

## Parameters and Arguments
```python
def add(a, b):
    return a + b

result = add(10, 20)
```
`a` and `b` are parameters. `10` and `20` are arguments.

## Default Arguments
```python
def connect(host, port=443):
    return f"{host}:{port}"
```

## Keyword Arguments
```python
connect(port=8080, host="localhost")
```

## return
`return` sends a value back to the caller and ends the function.

## Company Use
Functions often return structured values that other layers use.

## Common Mistakes
- Printing instead of returning when the caller needs the result
- Mutable default arguments such as `items=[]`

Safer:
```python
def add_item(item, items=None):
    if items is None:
        items = []
    items.append(item)
    return items
```

## Interview Questions
1. Parameter vs argument?
2. `print()` vs `return`?

## Practice
Write a function that returns annual salary from monthly salary.