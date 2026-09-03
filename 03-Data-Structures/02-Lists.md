# Lists

Lists are ordered and mutable collections.

```python
skills = ["Python", "AWS", "Linux"]
```

## Common Methods
```python
skills.append("SQL")
skills.remove("Linux")
print(skills[0])
```

## Looping
```python
for skill in skills:
    print(skill)
```

## Copying
```python
new_list = skills.copy()
```
Avoid accidental shared references when you need an independent list.

## Company Use
Batches, records, task queues, API results, ordered collections.

## Common Mistakes
- Index out of range
- Modifying a list while iterating over it carelessly
- Using a list when uniqueness is required

## Interview Questions
1. Why is a list mutable?
2. `append()` vs `extend()`?

## Practice
Create a list of services and remove every service marked as deprecated.