# 02 — Lists

## Simple Meaning
List ordered, mutable collection hai.

```python
skills = ["Python", "AWS", "SQL"]
```

## Access
```python
print(skills[0])
print(skills[-1])
```

## Add
```python
skills.append("Linux")
skills.insert(1, "Git")
```

## Remove
```python
skills.remove("SQL")
last = skills.pop()
```

## Update
```python
skills[0] = "Advanced Python"
```

## Length
```python
len(skills)
```

## Loop
```python
for skill in skills:
    print(skill)
```

## Useful Operations
```python
numbers = [4, 1, 9, 2]
print(sorted(numbers))
print(min(numbers))
print(max(numbers))
print(sum(numbers))
```

## Copy Important
Wrong mental model:
```python
a = [1, 2]
b = a
b.append(3)
```
Both references same list ko point karte hain.

Independent shallow copy:
```python
b = a.copy()
```

## Company Use
API se records often list me aate hain:
```python
servers = [
    {"name": "api-1", "status": "up"},
    {"name": "api-2", "status": "down"},
]
```

## Interview
- List mutable hai.
- `append()` one item add karta hai.
- `extend()` iterable ke items add karta hai.
- `remove()` value se; `pop()` index/item remove-return karta hai.

## Practice
1. Skills add/remove.
2. Largest number.
3. Duplicate count.
4. Active servers filter.
5. List copy behavior test.
