 # Introduction-to-Computer-Programming-Python-and-C-
## 1. setting up Dev environments for Python and C.
✅ 1. Setting Up a Python Development Environment
🛠 Tools Required:
Python Interpreter

Code Editor / IDE

Package Manager (pip or conda)

Virtual Environment (optional but recommended)

🔧 Steps:
Step 1: Install Python
Download from python.org

During installation, check the box that says "Add Python to PATH".

Confirm installation with:

```
python --version
```
Step 2: Install a Code Editor / IDE
Recommended:

VS Code

PyCharm

Step 3: Set Up a Virtual Environment (Optional but best practice)
```
# Create a virtual environment
python -m venv env
```
# Activate on Windows
.\env\Scripts\activate

# Activate on macOS/Linux
source env/bin/activate
Step 4: Install Python Packages
```
pip install numpy flask requests  # Example packages
```
Step 5: Install Python Extension in VS Code
Search “Python” in the Extensions panel

Install the official one by Microsoft

✅ 2. Setting Up a C Development Environment
🛠 Tools Required:
C Compiler (GCC or Clang)

Editor / IDE

Build tools (optional but useful)

🔧 Steps:
Step 1: Install a C Compiler
Windows:

Install MinGW-w64

Add bin/ folder to PATH

Confirm with:

```
gcc --version
```
macOS:

Install Xcode Command Line Tools:

```
xcode-select --install
Linux (Ubuntu/Debian):
```
```
sudo apt update
sudo apt install build-essential
```
Step 2: Install Code Editor / IDE
Recommended:

VS Code

CLion

Code::Blocks

Step 3: Configure Build and Run
In VS Code:

Install the C/C++ extension by Microsoft

Create a tasks.json and launch.json in the .vscode/ folder for build and debug configuration.

Step 4: Compile and Run Code
```
# Compile
gcc main.c -o main

# Run
./main
```
📁 Optional Tools for Both:
Git for version control

Docker for containerized environments

Jupyter for Python (use pip install notebook)

Make or CMake for C project management
   
## 2. "Hello World!" in Python and C

🐍 Python Version
```
# hello.py

print("Hello World!")
```
▶️ Run it:
```
python hello.py
```
💻 C Version
```
// hello.c

#include <stdio.h>

int main() {
    printf("Hello World!\n");
    return 0;
}
```
▶️ Compile and Run:
```
gcc hello.c -o hello
./hello
```
---
## Week 2: Data Types, Variables & Expressions
Primitive types, strings, arrays, memory model

Strong vs. weak typing

Immutable vs. mutable data

🧪 Lab: Type coercion experiments in JS vs. Python
---
## Week 3: Control Flow & Logic
Conditionals (if, switch)

Loops (for, while, recursion intro)

Boolean logic & short-circuiting

🧪 Assignment: Build a basic calculator or logic gate simulator
---
## Week 4: Functions & Modularization
Function definition and invocation

Scope & closures

Higher-order functions

🧪 Lab: Implement a mini math library (factorial, fibonacci, etc.)
---
## Week 5: Data Structures I
Arrays, Lists, Tuples, Dictionaries, Sets

Complexity analysis (Big-O basics)

🧪 Assignment: Frequency counter / simple search tool
---
## Week 6: Object-Oriented Programming (OOP)
Classes, Objects, Encapsulation

Inheritance, Polymorphism, Method overriding

Composition vs. Inheritance

🧪 Project: Build a simple role-playing game engine
---
## Week 7: Error Handling & Debugging
Syntax vs. semantic errors

Try/except blocks, assertions

Debugging with tools (pdb/gdb)

🧪 Lab: Debugging intentionally broken code
---
## Week 8: File I/O & Working with External Data
Reading/writing to files (JSON, CSV, XML)

APIs and basic networking

🧪 Lab: Read JSON weather data & parse into program
---
## Week 9: Recursion & Algorithm Design
Recursion vs. iteration

Call stack and tail recursion

Divide and conquer

🧪 Assignment: Solve merge sort, binary search recursively
---
## Week 10: Functional Programming Concepts
Pure functions, immutability, map/reduce/filter

Lambda calculus overview

🧪 Lab: Functional problems using Python or Haskell
---
## Week 11: Advanced Data Structures
Stacks, Queues, Trees, Graphs

Abstract Data Types (ADTs)

🧪 Assignment: Implement a basic graph traversal algorithm
---
## Week 12: Memory, Pointers & Low-Level Thinking
Memory layout, pointers (C), dynamic memory allocation

Garbage collection

🧪 Lab: Build a linked list in C or simulate memory usage
---
## Week 13: Testing & Software Quality
Unit tests, assertions, TDD principles

Linting, style guides, documentation

🧪 Lab: Add tests to previous assignments using pytest or JUnit
---
## Week 14: Capstone Project & Presentation
Build a mini-project (e.g., expense tracker, CLI chatbot, game)

Version control (Git/GitHub)

Peer review + presentation

🧪 Final Submission + Reflection
---
🧠 Supplementary Concepts (Optional Seminars)
Ethics in software development

Introduction to concurrency

Secure coding practices


