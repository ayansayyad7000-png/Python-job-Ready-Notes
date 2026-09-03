# 01 — Python + SQL with SQLite

SQLite Python standard library me available hai.

```python
import sqlite3

connection = sqlite3.connect("company.db")
cursor = connection.cursor()
```

Create table:
```python
cursor.execute("""
CREATE TABLE IF NOT EXISTS employees (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    role TEXT NOT NULL
)
""")
connection.commit()
```

Insert safely:
```python
cursor.execute(
    "INSERT INTO employees (name, role) VALUES (?, ?)",
    ("Ayan", "Platform"),
)
connection.commit()
```

Read:
```python
cursor.execute("SELECT id, name, role FROM employees")
for row in cursor.fetchall():
    print(row)
```

Update/Delete:
```python
cursor.execute("UPDATE employees SET role=? WHERE id=?", ("AI Platform", 1))
cursor.execute("DELETE FROM employees WHERE id=?", (1,))
connection.commit()
```

Close:
```python
connection.close()
```

## Company Note
Production may use PostgreSQL/MySQL + ORM, but CRUD/transaction concepts same foundation hain.
