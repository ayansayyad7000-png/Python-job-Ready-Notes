# 01 — Strings

## Simple Meaning
String text data hai.

```python
name = "Ayan Sayyad"
```

## Indexing
```python
print(name[0])   # A
print(name[-1])  # d
```

## Slicing
```python
text = "Python"
print(text[0:3])   # Pyt
print(text[::-1])  # nohtyP
```

Rule:
```text
[start : stop : step]
stop index include nahi hota.
```

## Useful Methods
```python
message = "  Python Job Ready  "

print(message.strip())
print(message.lower())
print(message.upper())
print(message.replace("Python", "SQL"))
```

Other useful methods:
```python
text.startswith("Py")
text.endswith("on")
text.find("th")
text.count("o")
text.split()
"-".join(["aws", "python"])
```

## Strings Are Immutable
```python
name = "Ayan"
# name[0] = "R"  # TypeError
```

New string create karo instead.

## Company Use
Input cleanup:
```python
email = input("Email: ").strip().lower()
```

Log parsing, API text, file names, validation—all me strings important hain.

## Interview
- String immutable hai.
- `strip()` whitespace remove karta hai.
- `split()` string → list.
- `join()` list of strings → one string.

## Practice
1. String reverse.
2. Vowel count.
3. Email lowercase/strip.
4. First and last character.
5. Words count using `split()`.
