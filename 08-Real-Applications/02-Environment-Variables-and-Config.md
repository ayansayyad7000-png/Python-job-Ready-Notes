# Environment Variables and Configuration

Do not hard-code secrets or environment-specific values in source code.

```python
import os

api_key = os.getenv("API_KEY")
environment = os.getenv("APP_ENV", "dev")
```

## .env Files
For local development, projects often use a `.env` file with a library such as `python-dotenv`.

```text
API_URL=https://example.com
APP_ENV=dev
```

Never commit real secrets.

## Config Pattern
Keep configuration separate from business logic.

```python
from dataclasses import dataclass

@dataclass
class Settings:
    environment: str
    api_url: str
```

## Company Use
Different values for local, test, staging, and production environments.

## Common Mistakes
- Committing `.env`
- Printing secrets in logs
- Using one giant unvalidated config dictionary

## Interview Question
Why should secrets come from environment variables or a secret manager?