# Regular Expressions (Regex)

Regex matches patterns in text.

```python
import re

text = "error code 503"
match = re.search(r"\d{3}", text)
if match:
    print(match.group())
```

## Common Functions
```python
re.search()
re.match()
re.findall()
re.sub()
```

## Raw Strings
Regex patterns usually use raw strings:
```python
pattern = r"\d+"
```

## Company Use
Log parsing, validation, extracting IDs, cleaning text.

## Common Mistakes
- Using regex for problems a simple string method solves better
- Overly complex patterns that nobody can maintain

## Interview Questions
1. `search()` vs `match()`?
2. Why use raw strings?

## Practice
Extract all IPv4-like values from a log string, then validate them separately.