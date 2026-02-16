# Lab Report 5: Advanced Data Structures (Sets & Dictionaries)
**Course:** Computer Science 101  
**Subject:** Analysis of Unordered and Mapped Collections in Python

---

## 1. Executive Summary
This report details the technical exploration of Python’s non-linear data structures: **Sets** and **Dictionaries**. The experiment focuses on understanding memory efficiency, data uniqueness, and key-value mapping—elements critical for optimized data retrieval and mathematical set theory applications.

## 2. Experimental Objectives
* To implement and verify **mathematical set operations** (Union, Intersection, Difference).
* To evaluate the performance of **Key-Value mapping** for data storage.
* To practice defensive programming using the `.get()` method and type-specific constructors.
* To utilize **Jupyter Notebook** and **Google Colab** for cloud-based execution.

---

## 3. Technical Theory: Sets

### 3.1 Characteristics
A **Set** is a collection that is both **unordered** and **unindexed**. Its primary constraint is the enforcement of **uniqueness**, where any duplicate entry is discarded during instantiation. 



[Image of Venn diagram showing Set Union, Intersection, and Difference]


### 3.2 Mathematical Operations
Sets in Python are optimized for high-speed logical comparisons:
* **Union (`|`):** Merges all distinct elements from two collections.
* **Intersection (`&`):** Identifies mutual elements; used frequently in "Mutual Friend" algorithms.
* **Difference (`-`):** Isolates elements unique to the primary set; used in recommendation engines (e.g., "Songs you haven't heard").
* **Symmetric Difference (`^`):** Captures elements present in either set, but excludes those present in both.

---

## 4. Technical Theory: Dictionaries

### 4.1 Architecture
A **Dictionary** is a hashed structure storing data in `key:value` pairs. Unlike lists, which require $O(n)$ time to find an element, dictionaries provide near-constant time $O(1)$ lookup speeds.



### 4.2 Data Retrieval Methods
The experiment compared two primary methods of data access:
1.  **Bracket Notation `[]`:** Direct access. Efficient but high-risk (triggers `KeyError` if the key is missing).
2.  **`.get()` Method:** Secure access. Returns `None` or a specified default value if the key is absent, preventing program crashes.

### 4.3 Nested Structures
The study included **Nested Dictionaries**, where a value is itself another dictionary. This creates a tree-like hierarchy essential for representing complex entities like User Profiles or JSON responses from APIs.

---

## 5. Practical Applications & Industry Use Cases

| Structure | Real-World Application | Technical Benefit |
| :--- | :--- | :--- |
| **Set** | **Search Filters** | Fast deduplication of search results (Amazon/Google). |
| **Set** | **Social Graphs** | Identifying mutual connections via Intersections. |
| **Dictionary** | **DNS Servers** | Mapping URLs (Keys) to IP Addresses (Values). |
| **Dictionary** | **Inventory Management** | Using Barcodes as unique keys for product metadata. |

---

## 6. Learning Outcomes
* **Data Integrity:** Confirmed that sets are the most efficient tool for "cleaning" datasets of duplicates.
* **Structural Mapping:** Mastered the use of dictionaries to create self-documenting code through labeling.
* **Efficiency:** Identified that hashed collections (Sets/Dicts) offer significantly faster access than sequential collections (Lists).

## 7. Conclusion
The experimental study of sets and dictionaries was successfully concluded. The verification of mathematical set operations and the implementation of robust dictionary lookups confirm their necessity in developing scalable, high-performance software.
