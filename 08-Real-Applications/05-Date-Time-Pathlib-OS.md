# Date/Time, pathlib and OS Tools

## datetime
```python
from datetime import datetime, timezone

now = datetime.now(timezone.utc)
print(now.isoformat())
```
Prefer timezone-aware datetimes for distributed systems.

## pathlib
```python
from pathlib import Path

path = Path("reports") / "daily.txt"
path.parent.mkdir(exist_ok=True)
path.write_text("ok", encoding="utf-8")
```

## os
```python
import os
print(os.getenv("APP_ENV"))
```

## Company Use
Log rotation, report filenames, file automation, environment access, cleanup scripts.

## Common Mistakes
- Using naive local timestamps in distributed systems
- Building paths manually with string concatenation

## Interview Questions
1. Why use `pathlib`?
2. Why are timezone-aware timestamps safer?