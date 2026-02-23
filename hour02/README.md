# 📘 Hour 2 – Algorithms, Abstraction & Introduction to C  
Part of **#24DaysOfCS50**

---

## 🎯 Overview

Hour 2 focused on moving from visual programming (Scratch) to formal computational thinking and C programming.

Core themes:
- Algorithms
- Conditionals
- Loops
- Functions
- Abstraction
- Binary logic
- Compiler fundamentals

---

# 🧠 1. Scratch – Thinking Before Syntax

Scratch was used to introduce logic without syntax overhead.

---

## 🔁 Event + Loop + Condition

```scratch
when green flag clicked
forever
    if touching mouse-pointer?
        play sound "Meow" until done
```

### Concepts:
- Event-driven programming
- Infinite loop (`forever`)
- Conditional branching
- Boolean evaluation

This mirrors how real applications continuously check system state.

---

## 🧩 Custom Functions with Parameters

```scratch
define meow (n times)
    repeat n
        play sound "Meow"
        wait 2 seconds
```

Called using:

```scratch
when green flag clicked
meow (3)
```

### Concepts:
- Abstraction
- Reusable logic
- Parameters controlling behavior
- Modularity

---

## 🔄 Separation of Logic and Control

```scratch
define meow
    play sound
    wait 1 second

when green flag clicked
repeat 3
    meow
```

This demonstrates:

- Function defines behavior
- Loop controls repetition

Separation of concerns is introduced early.

---

## 💬 User Input & String Concatenation

```scratch
when green flag clicked
ask "What's your name?" and wait
say join "hello," answer
```

Concepts:
- Input handling
- Stored response
- String concatenation
- Output formatting

---

# 📖 2. Algorithms – Phone Book Example

Problem:  
Is “John Harvard” in the phone book?

---

## ✏️ Pseudocode

```
1. Open phone book to middle
2. If name is on page → Done
3. If name comes earlier → Search left half
4. Else → Search right half
5. Repeat
```

This is **Binary Search**.

---

## 📈 Efficiency Insight

If input size doubles:
- 1000 pages → ~10 steps
- 2000 pages → ~11 steps

This follows:

```
O(log n)
```

Doubling input does not double runtime.

---

# 🧠 3. Abstraction

Abstraction hides complexity.

Example:

```c
printf("hello, world\n");
```

Behind this single line:
- Compiler translates to machine code
- OS handles input/output
- CPU executes binary instructions
- Transistors switch 0s and 1s

We only interact with the simplified interface.

---

# 🔢 4. Introduction to C

```c
#include <stdio.h>

int main(void)
{
    printf("hello, world\n");
}
```

### Breakdown:

- `#include <stdio.h>` → Standard library inclusion
- `int main(void)` → Entry point
- `{ }` → Scope block
- `printf()` → Output function
- `\n` → New line character

---

# 🔄 5. Compiler Concept

```
C Code → Compiler → Machine Code (Binary)
```

Computers do not understand C.  
They understand binary (0s and 1s).

The compiler translates human-readable code into machine instructions.

---

# 🔁 6. Input → Algorithm → Output Model

Fundamental computing structure:

```
Input → Algorithm → Output
```

All computation follows this model.

---

# 📍 7. Scratch Coordinate System

Scratch introduces Cartesian coordinates:

- (0, 0) → Center
- (240, 0) → Right edge
- (-240, 0) → Left edge
- (0, 180) → Top
- (0, -180) → Bottom

This connects programming to geometry and graphics systems.

---

# 🧩 8. Key Concepts Summary

| Concept        | Meaning |
|---------------|----------|
| Function      | Reusable block of logic |
| Parameter     | Input to function |
| Return Value  | Output from function |
| Side Effect   | Visible state change |
| Conditional   | Decision branching |
| Loop          | Repetition mechanism |
| Abstraction   | Hiding complexity |
| Algorithm     | Step-by-step solution |

---

# 🎓 Reflection

Hour 2 emphasizes:

- Thinking before coding
- Logic before syntax
- Abstraction before implementation
- Efficiency before optimization

Scratch is not “basic.”
It is a visual abstraction of real programming principles.

Revisiting these foundations reinforces structured thinking and teaching clarity.

---

## 🔖 Repository Structure

```
Hour2/
│── README.md
│── scratch-examples/
```

---

📌 Continuing the journey in #24DaysOfCS50
