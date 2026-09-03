# 05 — Date/Time, pathlib & OS

# datetime
```python
from datetime import datetime, timezone

now = datetime.now(timezone.utc)
print(now.isoformat())
```

Parse:
```python
created = datetime.strptime("2026-09-03", "%Y-%m-%d")
```

Format:
```python
created.strftime("%d-%m-%Y")
```

Production systems me timezone awareness important hai.

# pathlib
```python
from pathlib import Path

path = Path("data") / "report.csv"
print(path.exists())
```

Create folder:
```python
Path("logs").mkdir(exist_ok=True)
```

List files:
```python
for file in Path("data").glob("*.csv"):
    print(file)
```

# os
Environment/process-related utilities:
```python
import os
print(os.getenv("HOME"))
```

## Company Use
File automation, timestamped reports, scheduled jobs, config paths.
