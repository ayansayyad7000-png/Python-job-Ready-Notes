# Modules, Packages and pip

## Module
A Python file that can be imported.

`math_utils.py`:
```python
def add(a, b):
    return a + b
```

`main.py`:
```python
from math_utils import add
print(add(2, 3))
```

## Package
A directory containing related modules.

```text
app/
├── main.py
└── utils/
    ├── __init__.py
    └── validators.py
```

## pip
Installs third-party packages.
```bash
python -m pip install requests
python -m pip list
```

Save dependencies:
```bash
python -m pip freeze > requirements.txt
```

## Company Use
Real applications are split into modules and packages instead of one huge file.

## Common Mistakes
- Circular imports
- Installing packages globally
- Importing everything with `from module import *`

## Interview Question
Module vs package?