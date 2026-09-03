# 02 — Python Installation & Setup

## Goal

Is file ke baad tum Python install, version check aur basic program run kar paoge.

---

## Windows Setup

### Step 1 — Python Download

Official Python website se Python 3 install karo.

Installation ke time **Add Python to PATH** option tick karna important hai.

### Step 2 — Version Check

Command Prompt ya PowerShell open karo:

```bash
python --version
```

Expected output similar hoga:

```text
Python 3.x.x
```

Agar `python` command work nahi karta, try:

```bash
py --version
```

---

## Linux / Ubuntu Setup

Version check:

```bash
python3 --version
```

Install/update Python packages if needed:

```bash
sudo apt update
sudo apt install python3 python3-pip python3-venv -y
```

Check pip:

```bash
pip3 --version
```

---

## VS Code Setup

Recommended editor: **Visual Studio Code**.

Useful extension:

```text
Python — by Microsoft
```

Create file:

```text
hello.py
```

Code:

```python
print("Python setup is working")
```

Run from terminal:

```bash
python hello.py
```

Linux/macOS par:

```bash
python3 hello.py
```

---

## Interactive Python Shell

Terminal me:

```bash
python
```

Ya:

```bash
python3
```

Then:

```python
>>> 10 + 20
30
```

Exit:

```python
exit()
```

Interactive shell quick testing ke liye useful hai. Real project code `.py` files me likho.

---

## Important Commands

```bash
python --version
python app.py
pip --version
pip install package-name
```

Linux par commonly:

```bash
python3 --version
python3 app.py
pip3 --version
```

---

## PATH Kya Hota Hai?

PATH operating system ko batata hai executable program kaha installed hai.

Agar Python installed hai but terminal bolta hai:

```text
'python' is not recognized...
```

To usually PATH configuration issue ho sakta hai.

---

## Company Practice

Company projects me directly global Python packages install karna avoid kiya jata hai. Usually **virtual environment** use hota hai.

Example:

```bash
python -m venv .venv
```

Activate on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Linux/macOS:

```bash
source .venv/bin/activate
```

Virtual environments ko advanced section me detail me cover karenge.

---

## Common Mistakes

### Wrong Python Version

Project Python 3 require karta hai, lekin old interpreter select ho sakta hai. Always check:

```bash
python --version
```

### File Name Problem

Apni file ka naam built-in module ke naam par mat rakho.

Avoid:

```text
random.py
json.py
requests.py
```

Kyunki imports conflict kar sakte hain.

---

## Interview Questions

**Q1. `python` aur `python3` me difference?**  
System configuration ke according command name alag ho sakta hai. Goal correct Python 3 interpreter use karna hai.

**Q2. `pip` kya hai?**  
Python packages install/manage karne ka package manager.

**Q3. Virtual environment kyu use karte hain?**  
Har project ke dependencies isolate rakhne ke liye.

---

## Practice

1. Python version check karo.
2. `first.py` file banao.
3. Apna naam aur learning goal print karo.
4. Terminal se file run karo.
5. VS Code me correct Python interpreter select karna seekho.

---

## Quick Revision

```text
Python code file = .py
Run = python file.py
Packages = pip
Editor = VS Code
Project isolation = virtual environment
```

⬅️ Previous: [01 — What is Python?](01-What-is-Python.md)  
➡️ Next: [03 — Syntax, Comments & Indentation](03-Syntax-Comments-Indentation.md)
