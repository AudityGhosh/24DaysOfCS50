# 📘 CS50 – Hour 04  
## Comparison Programs, Increment Operators & Logical Conditions in C

> Part of my #24DaysOfCS50 journey  
> Hour 04 focuses on comparison logic, increment operators, user input handling, and structured decision flow.

---

# 🔹 1️⃣ Incrementing Variables in C

Understanding assignment and increment operators is foundational.

```c
int counter = 0;

counter = counter + 1;   // Explicit increment
counter += 1;            // Compound assignment
counter++;               // Post-increment operator
```

### Key Concepts

- `=` is the **assignment operator**
- `counter = counter + 1` updates the stored value
- `counter++` is shorthand for incrementing by 1
- These are essential for loops and counters (coming next)

---

# 🔹 2️⃣ Comparison Program (compare.c)

A simple program to compare two integers.

```c
#include <stdio.h>
#include <cs50.h>

int main(void)
{
    int x = get_int("What's x? ");
    int y = get_int("What's y? ");

    if (x < y)
    {
        printf("x is less than y\n");
    }
    else if (x > y)
    {
        printf("x is greater than y\n");
    }
    else
    {
        printf("x is equal to y\n");
    }
}
```

---

## 🧠 Logical Flow (Mental Model)

```
Start
   ↓
Input x, y
   ↓
Is x < y?
   ↓         ↓
 True      False
   ↓          ↓
Print       Is x > y?
"x < y"       ↓       ↓
              True    False
               ↓        ↓
        Print "x > y"  Print "x == y"
               ↓
              Stop
```

This visual branching reinforces how `if → else if → else` works internally.

---

# 🔹 3️⃣ Compilation & Execution

```bash
code compare.c
make compare
./compare
```

Example Run:

```
What's x? 1
What's y? 2
x is less than y
```

---

# 🔹 4️⃣ Character Input & Logical OR (agree.c)

This program evaluates user agreement using character comparison and logical operators.

```c
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    char c = get_char("Do you agree? ");

    if (c == 'y' || c == 'Y')
    {
        printf("Agreed\n");
    }
    else if (c == 'n' || c == 'N')
    {
        printf("Not agreed\n");
    }
}
```

---

## 🔍 Concepts Covered

### ✅ Character Data Type
- `char` stores a single character
- Characters are enclosed in single quotes: `'y'`

### ✅ Logical OR Operator

```
||
```

Used when **either condition can be true**.

Example:

```c
c == 'y' || c == 'Y'
```

Meaning:
- Accept lowercase OR uppercase input

---

# 🔹 5️⃣ Operators Reinforced

### Comparison Operators

| Operator | Meaning |
|----------|----------|
| `<` | Less than |
| `>` | Greater than |
| `==` | Equal to |

---

### Logical Operators

| Operator | Meaning |
|----------|----------|
| `||` | OR |
| `&&` | AND (not used here, but important) |

---

# 🔹 6️⃣ Structured Decision Thinking

Hour 04 strengthens:

- Comparison logic
- Branching structures
- Case handling
- Clean user interaction
- Flow-based reasoning

Programming is no longer just printing output —
it is evaluating conditions and choosing execution paths.

---

## Loops, Functions, Scope, Correctness & Design

Part of my **#24DaysOfCS50** journey  
Revisiting Computer Science fundamentals with a teaching-first perspective.

---

## 📌 Overview

Hour 4 also focuses on structured repetition, modular programming, and writing logically correct programs using:

- `while`, `for`, and `do while` loops  
- Infinite (forever) loops  
- Variable scope  
- Functions and function scope  
- Program correctness  
- Code design and style  

This is where programs begin to move from simple logic to structured systems.

---

# 🔁 Loops in C

## while Loop

Executes **as long as a condition is true**.

```c
int i = 0;
while (i < 3)
{
    printf("Hello\n");
    i++;
}
```



# 🔹 Key Learning Reflection

This hour reinforces a core principle:

> Programs become intelligent when they can compare, evaluate, and branch.

Key transitions:

- From simple conditions → multi-branch logic
- From integers → character evaluation
- From linear execution → decision
- Understanding increment operators also prepares for loops and iteration ahead.
- Correctness, design and style are important. 



# 🚀 Next Step : arrays.

#24DaysOfCS50 #CS50 #CProgramming #ComputerScience
