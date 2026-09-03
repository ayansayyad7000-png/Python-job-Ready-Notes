# 03 — Logging

## Why Not Only `print()`?
Logging level, timestamp, module, file output aur production observability deta hai.

```python
import logging

logging.basicConfig(
    level=logging.INFO,
    format="%(asctime)s %(levelname)s %(message)s",
)

logging.info("Application started")
logging.warning("CPU is high")
logging.error("Request failed")
```

## Levels
```text
DEBUG
INFO
WARNING
ERROR
CRITICAL
```

Module logger:
```python
logger = logging.getLogger(__name__)
```

Exception traceback:
```python
try:
    1 / 0
except ZeroDivisionError:
    logger.exception("Calculation failed")
```

## Security
Passwords, tokens, secret keys logs me mat print karo.

## Company Use
CloudWatch, ELK, Datadog etc. logs collect kar sakte hain.

## Interview
Logging structured operational information deta hai; level-based filtering possible hai.
