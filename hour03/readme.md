# 📘 CS50 – Hour 3  
## Control Flow, Operators & Conditional Logic in C

> Part of my **#24DaysOfCS50** learning journey.  
> Hour 3 focuses on how programs make decisions using operators and conditional statements in C.

---

## 🧭 Session Overview

In this hour, the focus shifted from writing simple programs to building **logic-driven programs** using:

- Arithmetic operators
- Comparison operators
- Logical operators
- `if`, `else if`, and `else` statements
- Basic command-line workflow
- Header files and libraries

This marks the transition from syntax to structured reasoning.

---

# 🔹 1️⃣ From Source Code to Execution (Recap)

### Example Program

```c
#include <stdio.h>

int main(void)
{
    printf("hello, world\n");
}
```

### What Happens Behind the Scenes?

```
Source Code (.c)
        ↓
Compiler (gcc / make)
        ↓
Machine Code (Binary: 0s and 1s)
        ↓
Program Output
```

### Common CS50 CLI Commands

```bash
code hello.c      # Create/edit file
make hello        # Compile
./hello           # Run (Mac/Linux)
ls                # List files
cd folder_name    # Change directory
mkdir folder      # Create directory
```

Understanding the CLI builds comfort with lower-level systems.

---

# 🔹 2️⃣ Operators in C

Operators allow us to compute values and evaluate conditions.

---

## ✅ Arithmetic Operators

| Operator | Description |
|----------|------------|
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Division |
| `%` | Modulus (Remainder) |

### Example

```c
int x = 10;
int y = 3;

printf("%i\n", x % y);   // Output: 1
```

---

## ✅ Comparison (Relational) Operators

Used for decision-making.

| Operator | Meaning |
|----------|----------|
| `==` | Equal to |
| `!=` | Not equal |
| `>`  | Greater than |
| `<`  | Less than |
| `>=` | Greater than or equal |
| `<=` | Less than or equal |

### Example

```c
if (x == 10)
{
    printf("x is ten\n");
}
```

---

## ✅ Logical Operators

Used to combine multiple conditions.

| Operator | Meaning |
|----------|----------|
| `&&` | Logical AND |
| `||` | Logical OR |
| `!`  | Logical NOT |

### Example

```c
if (x > 5 && x < 15)
{
    printf("x is between 5 and 15\n");
}
```

---

# 🔹 3️⃣ Conditional Statements

Conditional statements control the program's flow of execution.

---

## 🔸 Basic `if`

```c
if (condition)
{
    // Runs if condition is true
}
```

---

## 🔸 `if - else`

```c
if (condition)
{
    // Executes if true
}
else
{
    // Executes if false
}
```

### Example

```c
int age = 18;

if (age >= 18)
{
    printf("Eligible to vote\n");
}
else
{
    printf("Not eligible\n");
}
```

---

## 🔸 `if - else if - else`

Used when multiple conditions must be checked sequentially.

```c
int score = 85;

if (score >= 90)
{
    printf("Grade A\n");
}
else if (score >= 80)
{
    printf("Grade B\n");
}
else
{
    printf("Grade C or below\n");
}
```

---

# 🔹 4️⃣ Boolean Logic in C

In C:

- `0` → False  
- Any non-zero value → True  

### Logical Flow Model

```
Condition
   ↓
Evaluation (True / False)
   ↓
Branch Execution
```

This is the foundation of decision-making in programming.

---

# 🔹 5️⃣ Header Files & Libraries

```c
#include <stdio.h>
```

- Header files (`.h`) declare functions.
- `stdio.h` includes the declaration for `printf`.
- The compiler must know function declarations before compilation.

CS50 also introduces:

```c
#include <cs50.h>
```

Example:

```c
string name = get_string("What's your name? ");
```

---

# 🧠 Key Learning Reflection

Hour 3 represents a critical shift:

- From writing instructions  
- To designing decision-making logic  

Operators provide the tools.  
Conditionals provide the structure.  
Logic provides intelligence.

Revisiting these fundamentals strengthens structured problem-solving and improves clarity in both coding and teaching.

---

## 📂 Repository Structure

```
24DaysOfCS50/
 └── hour03/
      └── README.md
```

---

### 🚀 Continuing the Journey  
Next: Loops, iteration, and deeper control flow.

#24DaysOfCS50 #CS50 #ComputerScience #CProgramming
