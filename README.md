# Lux-Dev

## Week 1 & 2 Workings of a 3-Week Data Camp by Lux Dev Academy

---

<h2 align="center"> SQL 101: Introduction to Structured Query Language </h2>

### What is SQL?

- SQL stands for **Structured Query Language** and is a standard language for accessing and manipulating databases.
- It enables users to **access**, **manage**, and **manipulate** data in databases.

### Why Learn SQL?

- Develop **data management** and **retrieval** skills.
- High demand across industries that rely on databases for operations.
- Essential for **data analysts** to handle data effectively.
- Can be integrated with **R** and **Python** for advanced data analysis.
- SQL is **easy to learn** yet a **powerful tool** for managing data.

### Key Concepts in SQL

1. **Database**: A structured collection of data organized to store, retrieve, and manage data efficiently.
2. **Table**: Data arranged in rows and columns.
3. **Primary Key (PK)**: Unique identifier for a record in a table.
4. **Foreign Key**: A field in one table that refers to a primary key in another table.
5. **Data Types**: INT, VARCHAR, DATE, BOOLEAN.
6. **SQL Queries**: Interact with data using commands:
   - `SELECT`: Retrieves data from a database.
   - `INSERT`: Adds new data to a table.
   - `UPDATE`: Modifies existing data in a table.
   - `DELETE`: Removes data from a table.
7. **Filtering**: Use the `WHERE` clause to filter records based on specific conditions.
8. **Joins**: Combine data from multiple tables based on related columns:
   - `INNER JOIN`: Returns records with matching values in both tables.
   - `LEFT JOIN`: All records from the left table and matched records from the right.
   - `RIGHT JOIN`: All records from the right table and matched records from the left.
   - `FULL JOIN`: Returns records when there is a match in either table.
9. **Aggregate Functions**: Perform calculations on multiple rows of data:
   - `COUNT`: Counts the number of rows.
   - `SUM`: Adds up the values in a column.
   - `AVG`: Calculates the average value of a column.
   - `MIN/MAX`: Finds the minimum or maximum value in a column.
10. **GROUP BY**: Groups rows that share a common value.
11. **ORDER BY**: Sorts the result set in ascending or descending order.
12. **Constraints**: Ensure data integrity:
   - `NOT NULL`: Column cannot have null values.
   - `UNIQUE`: Ensures unique values.
   - `CHECK`: Validates that column values meet a specific condition.
   - `DEFAULT`: Sets a default value for a column.
13. **Normalization**: Organizes data to minimize redundancy by splitting it into smaller tables.
14. **Transactions**: Sequence of operations performed as a single unit of work:
   - `BEGIN TRANSACTION`: Start a transaction.
   - `COMMIT`: Save all changes made.
   - `ROLLBACK`: Undo changes.
15. **Indexes**: Used to speed up data retrieval.
16. **Views**: Virtual tables based on the result of an SQL query.

<h2 align="center"> Data Analysis Boot Camp Week 2 Assignment! </h2>

# Python Concepts Overview

This document covers essential Python concepts, including memory management, differences between data structures, list comprehensions, and copying methods.

---

### 1. Garbage Collection in Python

Garbage collection is an **automated memory management** process in Python that deletes objects when they are no longer in use.

**Memory Management Techniques**:
- Python uses a combination of **automatic garbage collection** and **reference counting**.
- **Reference Counting**: Every object in Python has a reference count, which tracks how many references point to that object.
- When the reference count drops to zero, the object becomes eligible for garbage collection.
- Python uses a **cyclic garbage collector** to detect and clean up circular references (i.e., objects referencing each other but otherwise unreachable).

---

### 2. Key Differences Between NumPy Arrays and Python Lists

| **Feature**           | **List**                        | **NumPy Array**                          |
|-----------------------|---------------------------------|------------------------------------------|
| **Mutability**         | Items can be changed or replaced| Items can be changed or replaced         |
| **Data Type**          | Can store multiple data types   | Stores only similar data types           |
| **Computation**        | Takes more space and time       | Efficient in terms of time and memory    |

**Advantages of NumPy Arrays in Numerical Computations**:
- **Less memory consumption** during computations.
- **Faster execution** for large data computations.

---

### 3. How Does List Comprehension Work in Python?

- **Iteration**: Python iterates over elements in the specified iterable (e.g., list or range).
- **Expression**: An operation is applied to each element (e.g., squaring a number).
- **Condition (optional)**: If specified, only elements satisfying the condition are included.
- **Collection**: The results are collected into a new list.

**Example**:
```python
squares = [x**2 for x in range(10)]
print(squares)
```

### 4. Shallow vs Deep Copying

#### Applications of Shallow Copying:
- Shallow copying is used when you want to create a new object but don't need to duplicate its elements.
- It is useful when working with **simple** or **non-nested data structures** (e.g., numbers, strings, tuples) or when you only need a **memory-efficient** way to create a copy without requiring full independence between the original and the copy.

#### Applications of Deep Copying:
- Deep copying is essential when you need to create a fully independent copy of an object, including all objects nested within it.
- It is commonly applied to **complex**, **nested data structures** (e.g., lists within lists, dictionaries) containing **mutable** elements like lists or custom objects.
- Deep copies ensure that modifications to the copied object **do not affect the original**, making it suitable for scenarios where full independence is required.

---

### 5. Differences Between Lists and Tuples

| **Feature**     | **List**                                        | **Tuple**                                      |
|-----------------|-------------------------------------------------|------------------------------------------------|
| **Mutability**  | Mutable, elements can be changed after creation | Immutable, elements cannot be changed once created |
| **Syntax**      | Lists are created using square brackets `[]`    | Tuples are created using parentheses `()`      |
| **Performance** | Lists are slower and consume more memory        | Tuples are faster and more memory-efficient    |

**Example 1: List**  
```python
my_list = [1, 2, 3, 4]
print(my_list)
```

**Example 2: Tuple**
```Python
my_tuple = (1, 2, 3, 4)
print(my_tuple)
```


