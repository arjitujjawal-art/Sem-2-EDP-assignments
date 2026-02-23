# 🔁 Types of Loop in Python

---

## 📖 Overview

Loops in Python are control flow statements that allow a block of code to be executed repeatedly based on a condition or over a sequence. They are essential for performing repetitive tasks efficiently and reducing code duplication.

Python provides simple, readable, and powerful looping structures that make it easy to iterate over data structures such as lists, tuples, strings, dictionaries, and ranges.

---

## 🎯 Aim

To study and understand the different types of loops in Python, their syntax, working principles, and practical applications in programming.

---

## 🛠 Tools Used

1. Python – Programming language used for implementation.
2. Jupyter Notebook / VS Code – Development environment for writing and running Python programs.

---

## 📚 Theory and Key Concepts

Python mainly provides two primary types of loops:

---

### 1️⃣ for Loop

The `for` loop is used to iterate over a sequence (such as a list, tuple, string, or range).

#### Syntax:

```python
for variable in sequence:
    # code block
```

#### Example:

```python
for i in range(5):
    print(i)
```

The `for` loop is typically used when the number of iterations is known in advance.

---

### 2️⃣ while Loop

The `while` loop executes a block of code as long as the given condition remains true.

#### Syntax:

```python
while condition:
    # code block
```

#### Example:

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

The `while` loop is used when the number of iterations depends on a condition rather than a fixed sequence.

---

## 🔑 Loop Control Statements

Python provides additional control statements to manage loop execution:

- `break` – Immediately terminates the loop.
- `continue` – Skips the current iteration and moves to the next iteration.
- `pass` – Acts as a placeholder and does nothing.
- `else` with loops – Executes when the loop completes normally (without encountering `break`).

---

## 🚀 Applications

Loops are widely used in:

- Iterating through lists and collections
- Data processing and analysis
- Searching and sorting algorithms
- Taking repeated user input
- File handling operations
- Automation scripts
- Game logic and simulations

---

## ✅ Advantages

- Reduces repetitive code
- Improves efficiency and readability
- Handles large datasets easily
- Flexible and simple syntax
- Essential for problem-solving in programming

---

## 🏁 Conclusion

Loops are fundamental constructs in Python programming. The `for` loop is ideal for sequence-based iteration, while the `while` loop is suitable for condition-based repetition.

A clear understanding of loop types and control statements enables developers to write efficient, scalable, and dynamic programs. Mastering loops is a key step toward becoming proficient in Python programming.
