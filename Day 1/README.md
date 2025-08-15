# Agentic AI Python Bootcamp – Day 1

## Table of Contents

- [1. Installing Python 3.13 and Visual Studio Code](#1-installing-python-313-and-visual-studio-code)
- [2. Why Python for AI and Agentic Systems?](#2-why-python-for-ai-and-agentic-systems)
- [3. Python Basic Syntax](#3-python-basic-syntax)
    - [Variables and Dynamic Typing](#variables-and-dynamic-typing)
    - [Print Statements](#print-statements)
    - [User Input](#user-input)
    - [Arithmetic Operators](#arithmetic-operators)
    - [Comments](#comments)
- [4. First Script: calculator.py](#4-first-script-calculatorpy)
- [5. Extended Calculator: More Operations](#5-extended-calculator-more-operations)
- [6. Good Coding Style (PEP 8) \& Naming](#6-good-coding-style-pep-8--naming)
- [7. Git: Initialize and Commit Your Work](#7-git-initialize-and-commit-your-work)

***

## 1. Installing Python 3.13 and Visual Studio Code

### Steps for Installation

**Python 3.13:**

- Visit [python.org/downloads](https://www.python.org/downloads/).
- Download the latest Python 3.13.x installer for your system.
- Run the installer; check “Add Python to PATH.”
- (Windows) Select default options, complete installation.

**Visual Studio Code:**

- Visit [code.visualstudio.com](https://code.visualstudio.com/).
- Download and install VS Code.
- Open VS Code, search for and install the “Python” extension (from Microsoft) for Python language support.

_Reference: Visual walkthroughs available on YouTube ([example](https://www.youtube.com/watch?v=WWWH2cBeLTc)) and in the official [VS Code docs](https://code.visualstudio.com/docs/python/python-tutorial)._[^1][^2][^3]

***

## 2. Why Python for AI and Agentic Systems?

- **Readable and simple syntax**: Easiest for beginners and professionals alike.
- Extensive **AI \& data science libraries**: Like NumPy, Pandas, TensorFlow, PyTorch.
- Great **community** and tons of learning resources.
- Python’s dynamic typing and quick prototyping speed up AI research and project delivery.
- Agentic AI (autonomous AI agents) often use Python for scripting logic and interface with tools.

***

## 3. Python Basic Syntax

### Variables and Dynamic Typing

Python variables do not require a declared type — types are inferred on assignment.

```python
x = 5        # integer
y = 2.5      # float
name = "Ana" # string
is_smart = True  # boolean
```

You can check a variable’s type with:

```python
print(type(x))     # <class 'int'>
print(type(name))  # <class 'str'>
```


***

### Print Statements

```python
print("Welcome to Python!")
print("The sum is:", x + 2)
```


***

### User Input

Always returns a string, so convert to int/float as needed.

```python
user_name = input("Enter your name: ")
age = int(input("Enter your age: "))
```


***

### Arithmetic Operators

| Operator | Meaning | Example | Result |
| :-- | :-- | :-- | :-- |
| + | Addition | 2 + 3 | 5 |
| - | Subtraction | 5 - 1 | 4 |
| * | Multiplication | 2 * 4 | 8 |
| / | Division (float) | 7 / 2 | 3.5 |
| // | Division (int) | 7 // 2 | 3 |
| % | Modulus (remainder) | 7 % 2 | 1 |
| ** | Exponentiation | 2 ** 3 | 8 |

_References \& practice: [W3Schools: Python Variables](https://www.w3schools.com/python/python_variables.asp), [Arithmetic Operators](https://www.geeksforgeeks.org/python/python-arithmetic-operators/)._[^11][^12][^13]

***

### Comments

- Single line: start with `#`
- Multi-line: triple single-quotes `''' ... '''`

```python
# This is a single-line comment

'''
This is a
multi-line comment
spanning several lines.
'''
```


***

## 4. First Script: calculator.py

Write a program that asks for two numbers and prints their sum.

```python
# calculator.py
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
sum = num1 + num2
print("Sum of", num1, "and", num2, "is", sum)
```


***

## 5. Extended Calculator: More Operations

```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

print("Addition:", num1 + num2)
print("Subtraction:", num1 - num2)
print("Multiplication:", num1 * num2)

# Handle division by zero error
if num2 != 0:
    print("Division:", num1 / num2)
else:
    print("Division: Cannot divide by zero.")
```


***

## 6. Good Coding Style (PEP 8) \& Naming

- Use descriptive variable names: `first_number` not `a`, `temp1`.
- Indent with **4 spaces** (never tabs).
- Write code in small, readable blocks.
- Place spaces around operators (`x + y`, not `x+y`).
- Add comments where reasoning may not be clear.

**Example:**

```python
# Good variable naming and coding style
first_number = int(input("Enter first number: "))
second_number = int(input("Enter second number: "))
total_sum = first_number + second_number  # Calculate the sum
print("The sum is:", total_sum)
```

*Reference: [PEP 8 Style Guide](https://peps.python.org/pep-0008/)*

***

## 7. Git: Initialize and Commit Your Work

- Open terminal (or VS Code terminal).

```bash
mkdir agentic-ai-python      # Create project directory
cd agentic-ai-python

# Optional: Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate    # On Windows: .venv\Scripts\activate

git init                     # Initialize git repository
cp path/to/calculator.py .   # Place your script in the folder
code .                       # Open in VS Code

git add calculator.py        # Stage your code
git commit -m "Day 1: Python basics and calculator"
```

- Next day, repeat `git add .` and `git commit -m "...your message..."` after new progress.

***

## Congratulations!

You’ve completed Day 1 — setup, Python basics, your first program, PEP 8 style, and version control.
Move to Day 2 once comfortable!

***
