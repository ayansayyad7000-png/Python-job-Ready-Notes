# Logging

Use logging instead of `print()` for production diagnostics.

```python
import logging

logging.basicConfig(level=logging.INFO)
logger = logging.getLogger(__name__)

logger.info("Service started")
logger.warning("CPU is high")
logger.error("Request failed")
```

## Log Levels
`DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`

## Include Context
```python
logger.info("Processing user_id=%s", user_id)
```

## Company Use
Troubleshooting, monitoring, audit trails, incident response.

## Security
Never log passwords, API keys, tokens, or sensitive personal data.

## Common Mistakes
- Logging every detail at `INFO`
- Swallowing exceptions without logs
- Using string concatenation for expensive log messages

## Interview Question
Why is logging better than print statements in production?