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
## 📘 Lesson: Data Types, Variables & Expressions in C
🧠 Objectives
By the end of this lesson, you will:

Understand primitive and derived data types in C

Declare and use variables correctly

Work with strings and arrays

Grasp how memory works in C

Understand C’s typing system

Learn the concept of mutability in C

1. 🧱 Primitive Data Types in C
These are the fundamental building blocks in C.

Data Type	Size (on 64-bit)	Example	Description
int	4 bytes	int x = 10;	Integer numbers
float	4 bytes	float pi = 3.14;	Single-precision decimal
double	8 bytes	double g = 9.81;	Double-precision decimal
char	1 byte	char c = 'A';	Single character
void	0 bytes	Used to define functions that return nothing	

⚠️ Note:
short, long, and long long offer size variations.

Use sizeof() to check memory size of types.

c
```
#include <stdio.h>

int main() {
    int x = 5;
    float f = 3.14;
    char ch = 'Z';

    printf("Size of int: %lu bytes\n", sizeof(x));
    printf("Size of float: %lu bytes\n", sizeof(f));
    printf("Size of char: %lu bytes\n", sizeof(ch));
    return 0;
}
```
## 2. 📦 Variables & Expressions
✅ Declaring Variables
```
int age = 25;
float salary = 45000.75;
char grade = 'B';
```
➕ Expressions
```
int a = 5, b = 3;
int sum = a + b;
Use +, -, *, /, % for arithmetic, and ==, !=, <, > for comparisons.
```
3. 🧵 Strings in C
C does not have a string type. Strings are character arrays ending with '\0' (null terminator).

✅ Declare a string:
```
char name[] = "Alice";
```
✅ Or manually:
```
char name[] = {'A', 'l', 'i', 'c', 'e', '\0'};
```
✅ Print string:
```
printf("Name: %s\n", name);
```
4. 📚 Arrays in C
Arrays store multiple values of the same type.

```
int scores[5] = {90, 80, 70, 60, 50};
```
Access using index:
```
printf("%d\n", scores[0]); // 90
```
Update:
```
scores[1] = 85;
⚠️ C does not check array bounds — accessing out-of-range elements may cause bugs.
```

5. 🧠 Memory Model in C
C variables are stored in memory locations (RAM).

Each variable occupies a contiguous block of memory.

Use pointers to access and manipulate memory directly.
```
int x = 10;
int *ptr = &x;  // Pointer to x

printf("Value: %d\n", *ptr);     // 10
printf("Address: %p\n", ptr);    // Memory address
```
6. 🧪 Strong vs. Weak Typing
C is statically typed: Variable types are declared and checked at compile time.

However, it allows type casting, which makes it weakly typed in some scenarios.

Example:
```
int i = 10;
float f = i; // Implicit conversion
```
⚠️ You can force a cast:

```
float pi = 3.14;
int approx = (int) pi;  // approx = 3
```
⚖️ Summary:
Feature	C supports?
Static typing	✅ Yes
Strong enforcement	❌ No
Implicit conversions	✅ Yes

7. 🔁 Mutable vs. Immutable Data
In C:
Primitive types (int, char, etc.) are mutable.

Strings (as char[]) are mutable, but string literals are immutable.
```
char name[] = "John";
name[0] = 'B';  // OK - modifies array

char *greet = "Hello";
// greet[0] = 'h'; ❌ - causes segmentation fault (immutable)
```
🔍 Recap
C has primitive types: int, float, char, etc.

Variables must be declared with a type.

Strings are char arrays.

Arrays store collections of values.

C allows low-level memory access via pointers.

It has weak typing behavior via casting.

Strings literals are immutable, arrays are mutable.

📝 Exercises
1. Declare variables of different types and print their sizes using sizeof().
2. Create a string and modify a character.
3. Initialize an integer array and print all elements.
4. Write an expression using int and float, observe implicit type conversion.
5. Try modifying a string literal and observe the error.
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


