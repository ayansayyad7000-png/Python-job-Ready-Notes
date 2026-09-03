# 03 — Tuples & Sets

# Tuple
Ordered and immutable collection.

```python
coordinates = (19.07, 72.87)
```

Access:
```python
print(coordinates[0])
```

Unpacking:
```python
lat, lon = coordinates
```

Use tuple jab values logically fixed hon.

# Set
Unique unordered collection.

```python
services = {"EC2", "S3", "EC2"}
print(services)
```

Duplicate remove ho jayega.

## Set Methods
```python
services.add("Lambda")
services.discard("S3")
```

## Set Operations
```python
a = {"Python", "AWS", "SQL"}
b = {"Python", "Linux"}

print(a & b)  # intersection
print(a | b)  # union
print(a - b)  # difference
```

## Company Use
Duplicate IDs remove:
```python
user_ids = [101, 101, 102, 103]
unique_ids = set(user_ids)
```

## Interview
- tuple immutable; list mutable.
- set unique values rakhta hai.
- set indexing support nahi karta.

## Practice
1. List duplicates remove.
2. Two skill sets common values.
3. Tuple unpack.
4. Union/intersection run karo.
