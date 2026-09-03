# 02 — Environment Variables & Config

## Why?
Secrets/settings code me hardcode nahi karne.

Bad:
```python
API_KEY = "real-secret"
```

Environment:
```python
import os

api_key = os.getenv("API_KEY")
region = os.getenv("AWS_REGION", "ap-south-1")
```

Required setting:
```python
if not api_key:
    raise RuntimeError("API_KEY is required")
```

## `.env`
Local development me `.env` common hai, but Git me commit nahi karna.

`.gitignore`:
```text
.env
.venv/
```

With `python-dotenv`:
```bash
pip install python-dotenv
```

```python
from dotenv import load_dotenv
load_dotenv()
```

## Config Pattern
```python
from dataclasses import dataclass
import os

@dataclass
class Settings:
    region: str = os.getenv("AWS_REGION", "ap-south-1")
```

## Company Use
Dev/staging/prod differences, credentials, endpoints, feature flags.
