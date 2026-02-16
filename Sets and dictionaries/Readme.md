# Experiment 5: Sets and Dictionaries in Python

A **Set** serves as an unordered repository for unique items, making it ideal for high-speed membership testing, removing redundancies from datasets, and performing standard algebraic set operations.

A **Dictionary** functions as an associative array or map, utilizing unique keys to store and retrieve corresponding values. This structure is engineered for efficient data management and rapid lookup performance.

### Aim:
To investigate and implement various operational methods for Sets and Dictionaries within the Python environment.

### Tools Used:
* **Google Colab** (Cloud-based development)
* **Jupyter Notebook** (Local execution)

### Theory:

## Sets in Python

In Python, a set is an optimized collection type that enforces uniqueness. Because sets are unordered, they lack indexing; elements are retrieved based on their value rather than a specific position. The primary constraint of a set is that while the collection itself is mutable, every individual element must be of an immutable data type.



[Image of Venn diagram showing set union, intersection, and difference]


**Creation of Set:**
* Sets are initialized using curly braces `{}` containing elements or via the `set()` constructor.
* To define an empty set, the `set()` function must be used, as empty curly braces `{}` are reserved for initializing dictionaries.

**Common Set Operations:**
Python utilizes specific operators to perform mathematical set logic:
* **Union (`|`):** Aggregates every unique element found across both sets.
* **Intersection (`&`):** Identifies and returns only the elements shared by both collections.
* **Difference (`-`):** Returns elements present in the leading set that do not exist in the second.
* **Symmetric Difference (`^`):** Collects elements that are present in either set, but excludes those present in both.

**Applications of Sets:**
* **Social Networking:** Calculating "Mutual Friends" through intersection operations.
* **Streaming Services:** Spotify generates personalized recommendations by identifying the "Difference" between a global library and a user's "Already Played" set.
* **E-commerce:** Implementing complex search filters using logical AND/OR operations on product attributes.

**Advantages of Sets:**
* **Data Sanitization:** Their inability to hold duplicates makes them the premier tool for cleaning "dirty" data.
* **Syntactic Conciseness:** Complex logical comparisons that would require nested loops in other structures can be performed in a single line of code.

## Dictionary in Python:
Dictionaries are built-in structures that implement a "Key-Value" mapping system. Data retrieval is achieved by referencing a specific key rather than an index number. 



In a dictionary, keys must be unique to prevent data collisions. If a duplicate key is assigned, Python updates the entry with the most recent value provided. Dictionaries also support **Nesting**, where values can consist of other dictionaries, enabling the creation of multi-layered, JSON-like data hierarchies.

**Creation of Dictionary:**
* Dictionaries are defined using `{key: value}` syntax or the `dict()` keyword.
* An empty dictionary is simply declared as `{}` or `dict()`.

**Accessing and Modifying Data:**
There are two primary paradigms for interacting with dictionary data:
* **Bracket Notation `[]`:** A direct access method that is efficient but will trigger a `KeyError` if the requested key is missing.
* **`.get()` Method:** A safer alternative for data retrieval that returns `None` (or a custom default) if the key is not found, preventing runtime crashes.

**Important Keywords in Dictionaries:**
* `keys()`: Generates a view object of all identifiers in the collection.
* `values()`: Provides a view of all stored data without their associated keys.
* `items()`: Returns a list-like object containing `(key, value)` tuples for every entry.

**Application of Dictionary:**
* **Network Infrastructure:** The Domain Name System (DNS) maps human-readable URLs to numeric IP addresses using a dictionary-style lookup.
* **Web Performance:** Dictionaries are used for "Caching," storing the results of heavy computations to speed up subsequent requests.
* **Logistics:** Barcode systems use the numeric code as a key to instantly pull product descriptions and pricing from a central database.

**Advantages of Dictionary:**
* **Data Labeling:** By using descriptive keys, the code becomes self-documenting and easier for other developers to interpret.
* **Memory Management:** Unlike arrays that require contiguous memory blocks, dictionaries use a sparse hash table approach, making them flexible for large datasets.

**Learning Outcomes:**
* Recognized that hashed collections (Sets/Dictionaries) offer significantly lower latency for data access than sequential Lists.
* Developed the ability to enforce data uniqueness using Sets and maintain structured, labeled relationships using Dictionaries.

**Conclusion:**
Through the successful execution and verification of these operations, the efficiency of Python’s advanced data structures in handling complex logic was confirmed.
