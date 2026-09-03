# Parameterized Queries and Transactions

## Safe Query
Never concatenate untrusted input into SQL.

Wrong:
```python
query = f"SELECT * FROM users WHERE name = '{name}'"
```

Better:
```python
cursor.execute("SELECT * FROM users WHERE name = ?", (name,))
```

Different database drivers use different placeholder styles.

## Transactions
A transaction groups operations that should succeed or fail together.

```python
with sqlite3.connect("app.db") as conn:
    conn.execute("UPDATE accounts SET balance = balance - ? WHERE id = ?", (100, 1))
    conn.execute("UPDATE accounts SET balance = balance + ? WHERE id = ?", (100, 2))
```

## Company Use
Payments, inventory, account changes, reliable multi-step writes.

## Interview Questions
1. Why parameterize SQL?
2. What is a transaction?
3. What is rollback?