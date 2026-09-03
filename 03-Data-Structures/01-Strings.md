# Strings

Strings store text.

```python
service = "payment-api"
```

## Useful Operations
```python
service.upper()
service.lower()
service.strip()
service.replace("api", "service")
service.split("-")
len(service)
```

## Indexing and Slicing
```python
text = "python"
print(text[0])
print(text[1:4])
```

Strings are immutable.

## Company Use
Parsing logs, cleaning API input, validation, file paths, messages.

## Common Mistakes
- Forgetting strings are immutable
- Using case-sensitive comparison without normalization

## Interview Questions
1. Are strings mutable?
2. What does `.strip()` do?

## Practice
Normalize `"  PROD-API  "` to lowercase without outer spaces.