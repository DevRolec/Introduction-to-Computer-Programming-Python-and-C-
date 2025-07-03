# 🧠 Module 1: Introduction to C Programming
## ✅ 1. What is C Programming?
C is a general-purpose, high-performance programming language developed in the early 1970s. It provides low-level access to memory and is widely used in system/software development, embedded systems, and operating systems (like Unix/Linux).

🔑 Key Features of C:
Procedural language

Statically typed

Compiled language

Close to hardware (low-level manipulation)

## 🏛 2. Brief History of C
Year	Milestone
1969	Ken Thompson developed the B language at Bell Labs.
1972	Dennis Ritchie developed the C language based on B.
1978	First edition of The C Programming Language book by Kernighan and Ritchie (K&R).
1989	ANSI C was standardized (also known as C89 or C90).
1999	C99 added new features like inline, new data types.
2011	C11 improved multithreading support.

🧠 C influenced many languages including C++, Java, C#, and Go.

## ⚙️ 3. The Compilation Process in C
💡 Flow:
```c
C Source Code (.c)
      ↓
Preprocessor (includes #includes, macros)
      ↓
Compiler (translates to assembly)
      ↓
Assembler (converts to machine code/object code)
      ↓
Linker (combines libraries into final executable)
      ↓
Executable File (.exe / a.out)
```
Example:
If you write hello.c, the compilation process is:

```c
gcc hello.c -o hello
./hello
```
## 🧱 4. Structure of a Basic C Program
Example: Hello World
```c
#include <stdio.h> // Preprocessor directive

int main() {       // Main function
    printf("Hello, World!\n");  // Output to screen
    return 0;       // Exit code
}
```
Breakdown:
#include <stdio.h> – includes standard input-output header

main() – entry point of the program

printf() – built-in function to display output

return 0; – signals successful execution

## 🛠 5. Setting Up an IDE for C Programming
Option 1: VS Code (Recommended for Beginners)
Steps:

Install VS Code

Install C/C++ Extension by Microsoft

Install GCC Compiler:

On Windows: Install MinGW

On Linux: sudo apt install build-essential

Create a .c file and write code.

Open terminal and compile: gcc file.c -o file && ./file

Option 2: Code::Blocks IDE
Download from www.codeblocks.org

Has built-in GCC support

Great for offline use

✍️ Practice Code Examples
➤ 1. Print Your Name
```c
#include <stdio.h>

int main() {
    printf("My name is Roland\n");
    return 0;
}
```
➤ 2. Add Two Numbers
```c
#include <stdio.h>

int main() {
    int a = 5, b = 10;
    int sum = a + b;
    printf("Sum is: %d\n", sum);
    return 0;
}
```
## 📝 Practice Test (Quiz & Code)
🔍 Part A: Multiple Choice
Who developed the C language?

-A) Ken Thompson

-B) Dennis Ritchie

-C) Bjarne Stroustrup

-D) James Gosling
→ Answer: B

What is the file extension for a C source file?

-A) .cpp

-B) .java

-C) .py

-D) .c
→ Answer: D

What does #include <stdio.h> do?

-A) Starts the program

-B) Compiles the code

-C) Includes standard input-output functions

-D) Links the file
→ Answer: C

🔍 Part B: Code Tracing
Question: What is the output of the following code?

```c
#include <stdio.h>

int main() {
    int x = 4;
    printf("x = %d\n", x);
    return 0;
}
```
Answer: x = 4

🔧 Part C: Hands-On Tasks
Write a C program that prints your school’s name.

Write a program that adds two integers entered by the user.

Modify the Hello World program to say: “Hello, Software Engineer!”
---
