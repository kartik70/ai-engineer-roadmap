# Python Fundamentals — 01: Python and JavaScript

## 1. What is Python?
Python is a general-purpose programming language used for backend development, automation, scripting, DSA, and AI engineering.

## 2. Python vs JavaScript

| JavaScript | Python |
|---|---|
| Node.js commonly executes JS on the server | CPython is the most common Python implementation |
| console.log() | print() |
| null | None |
| let/const | Direct variable assignment |
| npm | pip / uv |
| package.json | pyproject.toml |
| {} for code blocks | Indentation |

## 3. How Python executes code
- Python is commonly described as an interpreted language.
- CPython compiles source code into bytecode.
- The Python virtual machine executes the bytecode.
- This is why Python is not simply executing raw source code line by line.

## 4. First Python program

```python
name = "Kartik"
experience = 3

print("Hello", name)
print("Experience:", experience)
```

Run the program:
```bash
python3 main.py
```

## 5. Important takeaways
- Python variables do not require let or const.
- Semicolons are generally unnecessary.
- Indentation defines code blocks.
- Python uses None instead of JavaScript's null.
- Python type hints are not enforced at runtime by default.

## 6. Interview questions
1. Is Python interpreted or compiled?
   - CPython compiles source code to bytecode, which is executed by its virtual machine.
2. What is the difference between Node.js and CPython?
   - They are different language runtimes. Node.js runs JavaScript using V8, while CPython is the standard implementation of Python.
3. Does Python require semicolons?
   - No, they are generally unnecessary.
4. What defines a code block in Python?
   - Indentation.

## 7. My doubts and learnings
- Add questions and explanations from the tutorial here.

## 8. Practice
- [x] Write and run a Python script.
- [x] Declare variables and print their values.
- [x] Explain how Python executes code.