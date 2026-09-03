# Python + SQLite CRUD

SQLite is useful for learning SQL integration and small local applications.

```python
import sqlite3

with sqlite3.connect("app.db") as conn:
    conn.execute(
        "CREATE TABLE IF NOT EXISTS users (id INTEGER PRIMARY KEY, name TEXT)"
    )
    conn.execute("INSERT INTO users(name) VALUES (?)", ("Ayan",))

    rows = conn.execute("SELECT id, name FROM users").fetchall()
    print(rows)
```

## CRUD
- Create: `INSERT`
- Read: `SELECT`
- Update: `UPDATE`
- Delete: `DELETE`

## Company Use
The same application patterns apply to PostgreSQL/MySQL through different drivers or ORMs.

## Common Mistakes
- Building SQL with f-strings
- Forgetting transactions
- Mixing database logic everywhere in the codebase

## Interview Question
What does CRUD stand for?