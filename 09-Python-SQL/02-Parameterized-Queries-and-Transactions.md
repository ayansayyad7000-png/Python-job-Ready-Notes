# 02 — Safe Queries & Transactions

## Never Build SQL With User String Concatenation
Bad:
```python
query = "SELECT * FROM users WHERE name='" + name + "'"
```

SQL injection risk.

Use parameters:
```python
cursor.execute("SELECT * FROM users WHERE name = ?", (name,))
```

Different DB libraries placeholder style change kar sakti hain.

## Transaction
Related operations all succeed or all rollback.

```python
try:
    cursor.execute("UPDATE accounts SET balance=balance-100 WHERE id=?", (1,))
    cursor.execute("UPDATE accounts SET balance=balance+100 WHERE id=?", (2,))
    connection.commit()
except Exception:
    connection.rollback()
    raise
```

## Company Concepts
- parameterized query
- transaction
- commit
- rollback
- connection lifecycle
- indexes/query performance (SQL topic)

## Interview
Parameterized queries values ko SQL code se separate rakh kar injection risk reduce karti hain.
