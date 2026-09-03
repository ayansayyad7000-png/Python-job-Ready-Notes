# 07 — Operators

## Arithmetic
```python
print(10 + 3)
print(10 - 3)
print(10 * 3)
print(10 / 3)   # division
print(10 // 3)  # floor division
print(10 % 3)   # remainder
print(2 ** 3)   # power
```

## Comparison
```python
age >= 18
status == "active"
```

## Logical
```python
age >= 18 and has_id
is_admin or is_owner
not is_blocked
```

## Membership
```python
"Python" in skills
```

## Identity
`is` checks object identity, not value equality.
```python
a == b
#a is b  # different meaning
```
Use `is None` for `None` checks.

## Company Use
Operators power validation rules, access checks, filtering, calculations, and business logic.

## Common Mistakes
- Using `=` instead of `==`
- Using `is` instead of `==` for normal value comparison

## Interview Questions
1. `/` vs `//`?
2. `==` vs `is`?
3. What does `%` return?

## Practice
Write an expression that checks whether a user is active and has age 18 or above.