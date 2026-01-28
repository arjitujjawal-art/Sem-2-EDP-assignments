# Experiment 4: Operations on Tuples

## 📝 Overview
This project explores the **Tuple** data structure in Python. While tuples are similar to lists in their ability to store multiple data types in a sequence, they possess the unique property of **immutability**, making them essential for specific use cases in software development.

---

## 🎯 Aim
To study and implement various operations on tuples and understand the functional differences between mutable and immutable sequences.

## 🛠️ Tools Used
* **Jupyter Notebook** or **Google Colab**

---

## 📖 Theory & Concepts

### 1. What is a Tuple?
A tuple is a built-in Python data type used to store a finite, ordered sequence of elements. It acts as a dynamic placeholder for multiple data types (Integers, Strings, Floats, etc.).



### 2. Types of Tuples
* **Empty Tuple:** Represented by empty parentheses `()`. It contains no elements or spaces.
* **Filled Tuple:** Contains one or more elements. Even a single-element tuple requires a trailing comma (e.g., `(5,)`) to be recognized by the interpreter.

### 3. Key Properties
* **Representation:** Elements are enclosed in parentheses `()` and separated by commas.
* **Indexing:** Items are accessed via zero-based indexing, exactly like lists.
* **Immutability:** Once a tuple is created, its elements cannot be added, removed, or modified.

---

## 🔄 Operations & Comparison

### Shared Operations (Lists & Tuples)
These operations work on both types because they do not modify the underlying data:
* **Slicing:** Accessing a specific range of elements (e.g., `tup[1:4]`).
* **Membership:** Using the `in` operator to check if an element exists.
* **Length:** Using the `len()` function to count elements.

### Restricted Operations (Why Tuples are Different)
Because tuples are immutable, the following list methods **will raise an error** if attempted on a tuple:
❌ `.append()` | ❌ `.insert()` | ❌ `.remove()` | ❌ `.pop()` | ❌ `.sort()`

---

## 💡 Practical Insights

### Data Conversion
* **Type Casting:** We can convert other iterables (like lists) into tuples using the `tuple()` constructor.
* **Non-Iterables:** Data types like `int` or `float` cannot be converted directly into a tuple because they cannot be iterated over.

### Real-World Applications
1.  **Data Integrity:** Used when data should remain constant throughout the program lifecycle.
2.  **Graphics/UI:** Defining RGB color values (e.g., `Red = (255, 0, 0)`).
3.  **Geo-Mapping:** Storing specific GPS coordinates (Latitude, Longitude).

---

## ✅ Advantages
* **Performance:** Tuples are faster to iterate through than lists.
* **Memory Efficiency:** They consume less RAM compared to lists.
* **Hashability:** Because they are immutable, tuples can be used as keys in dictionaries.

## 🏁 Conclusion
Through this experiment, I have successfully executed basic tuple operations. The primary takeaway is that while tuples share a similar syntax with lists, their **immutability** provides a layer of security and efficiency that is vital for structured data handling.

---
