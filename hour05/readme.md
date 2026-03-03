# 📘 CS50 – Hour 05

## Loops, Nested Loops, User Input & Floating-Point Precision in C

This repository contains practice implementations from **CS50 Hour 05**, focusing on loop structures, pattern printing, user input handling, and floating-point precision behavior in C.

---

# 🔹 1️⃣ Basic Output in C

```c
#include <stdio.h>

int main(void)
{
    printf("????\n");
}
```

### ✅ Concept

* `\n` creates a new line.
* `printf()` prints formatted output to the console.

---

# 🔹 2️⃣ Loop-Based Character Printing

## ❌ Vertical Output (Incorrect for horizontal pattern)

```c
for (int i = 0; i < 4; i++)
{
    printf("?\n");
}
```

**Output:**

```
?
?
?
?
```

## ✅ Horizontal Output (Correct)

```c
for (int i = 0; i < 4; i++)
{
    printf("?");
}
printf("\n");
```

**Output:**

```
????
```

### 🎯 Key Learning

* Placing `\n` inside the loop prints vertically.
* Placing `\n` outside prints horizontally.

---

# 🔹 3️⃣ Nested Loops – Printing a 3×3 Grid

```c
#include <stdio.h>

int main(void)
{
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            printf("#");
        }
        printf("\n");
    }
}
```

**Output:**

```
###
###
###
```

### 🎯 Key Learning

* Outer loop → Controls rows
* Inner loop → Controls columns
* Nested loops create 2D structures.

---

# 🔹 4️⃣ Simple Calculator Using User Input

```c
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int x = get_int("What's x? ");
    int y = get_int("What's y? ");

    int z = x + y;

    printf("Sum: %d\n", z);
}
```

### 🎯 Key Learning

* `get_int()` collects user input.
* `%d` is used for integer formatting.
* Variables store intermediate results.

---

# 🔹 5️⃣ Infinite Loop with Condition-Based Exit

```c
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    long dollars = 1;

    while (true)
    {
        char c = get_char("Double it? (y/n): ");

        if (c == 'y' || c == 'Y')
        {
            dollars *= 2;
            printf("Dollars: %li\n", dollars);
        }
        else
        {
            break;
        }
    }
}
```

### 🎯 Key Learning

* `while(true)` creates an infinite loop.
* `break` exits the loop.
* Logical OR operator: `||`

---

# 🔹 6️⃣ Floating-Point Imprecision

```c
#include <stdio.h>

int main(void)
{
    printf("%.20f\n", 0.1 + 0.2);
}
```

**Possible Output:**

```
0.30000000000000004441
```

### 🎯 Why This Happens

* Floating-point numbers are stored in binary.
* Some decimal values cannot be represented exactly.
* This causes small precision errors.

---

# 📚 Concepts Covered

* `for` loops
* Nested loops
* Infinite loops
* Conditional statements
* User input handling
* Arithmetic operations
* Floating-point precision limitations

---

# 🚀 Learning Outcome

By completing this practice:

* I can construct pattern-based outputs using nested loops.
* I understand loop control flow.
* I can handle user input and perform arithmetic operations.
* I recognize floating-point precision limitations in C.

---

📌 *Part of my CS50 structured learning journey.*
