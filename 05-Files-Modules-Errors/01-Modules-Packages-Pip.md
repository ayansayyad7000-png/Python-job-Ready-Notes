# 01 — Modules, Packages & pip

## Module
Ek `.py` file jisme reusable code ho.

`math_utils.py`:
```python
def add(a, b):
    return a + b
```

`app.py`:
```python
from math_utils import add
print(add(2, 3))
```

## Import Styles
```python
import math
from math import sqrt
import math as m
```

Avoid wildcard in production:
```python
from module import *
```

## Package
Related modules ka folder, often package structure me `__init__.py` hota hai.

## pip
Third-party packages install:
```bash
pip install requests
```

List:
```bash
pip list
```

Freeze:
```bash
pip freeze > requirements.txt
```

Install project dependencies:
```bash
pip install -r requirements.txt
```

## `if __name__ == "__main__"`
```python
def main():
    print("App started")

if __name__ == "__main__":
    main()
```

File directly run ho to `main()` execute; import hone par automatically nahi.

## Company Use
Projects modules/packages me divide hote hain: `api`, `services`, `utils`, `models`.

## Interview
- module = Python file.
- package = modules ka package/folder.
- pip = package installer.
- requirements.txt dependencies record karta hai.
