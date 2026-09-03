# 04 — Regular Expressions (Regex)

## Simple Meaning
Text pattern search/validation.

```python
import re

text = "Order ID: 12345"
match = re.search(r"\d+", text)
print(match.group())
```

## Common Tokens
```text
\d digit
\w word char
\s whitespace
. any char
+ one or more
* zero or more
^ start
$ end
```

## Find All
```python
numbers = re.findall(r"\d+", "cpu=80 memory=65")
```

## Simple Email-Like Check
```python
pattern = r"^[^\s@]+@[^\s@]+\.[^\s@]+$"
```

Regex useful hai, but complex validation ke liye specialized libraries better ho sakti hain.

## Company Use
Logs parsing, IDs extraction, text cleanup, validation.
