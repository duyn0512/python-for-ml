# PYTHON FOR DATA SCIENE

This document systematizes core knowledge, syntax, and programming concepts required

## WEEK 1: PYTHON CORE FOR DATA PROCESSING

### 1. Primitive Types & Casting

- **5 Primitive data types**
  - `int` - Integer: Whole numbers
  - `float` - Floating-point: Decimal numbers
  - `str` - String: Text characters
  - `bool` - Boolean: Logical True/False
  - `None` - NoneType: Represents missing or null values
- **Type Casting:** Converting between data types.
- **Mutability & Imutability**
  - **Inmutable - Unchangeable in-place:** `int`, `float`, `str`, `bool`, `tuple`.
  - **Mutable - Changeale in-place:** `list`, `dict`, `set`.

### 2. Control Flow
- **Conditional Statements:** `if/ elif/ else` logical operators `and`, `or`, `not`, `in`, `is`.
- **Basic Loops:**
  - `for`: Interates over sequences
  - `while`: Repeats while condition is False
- **Loop Helper Functions:**
  - `range(start, stop, step)`: Generates a sequence of numbers
  - `enumerate(iterable)`: Returns both index and value during iteration
  - `zip(list1, list2, ...)`: Pairs elements from multiple iterables in parallel

### 3. Core Data Structues
- **Indexing & Slicing:**
  - `arr[i]`: Accesses element at index `i` (negative indices like `arr[-1]` count from the end).
  - `arr[start:stop:step]`: Extracts a sub-sequence.
  - `arr[::-1]`: Shortcut to reverse a sequence.

- **Comparison of Core Data Structures:**

| Structure | Syntax | Core Characteristics | Primary Use Cases |
| :--- | :---: | :--- | :--- |
| **`list`** | `[...]` | Ordered, Duplicates allowed, **Mutable** | Dynamic data sequences |
| **`tuple`** | `(...)` | Ordered, Duplicates allowed, **Immutable** | Fixed records, memory efficiency |
| **`dict`** | `{k: v}` | `Key: Value` pairs, Unique keys | Structured records, JSON objects |
| **`set`** | `{...}` | Unordered, **Unique elements only** | Deduplication, Set operations |

### 4. Comprehensions (Pythonic Shortcuts)
- **List Comprehension:** Filter and transform lists in a concise single line.
  - *Syntax:* `[EXPRESSION for ITEM in ITERABLE if CONDITION]`
- **Dict Comprehension:** Construct dictionaries programmatically.
  - *Syntax:* `{KEY: VALUE for ITEM in ITERABLE if CONDITION}`

## WEEK 2: FUNCTIONS, MODULES & ERROR HANDLING

### 1. Function Declaration & Execution
- **`def` Statement:** Defines a reusable block of code.
- **`return` Statement:** Exits a function and optionally passes back a value. If omitted, returns `None`.

### 2. Parameters & Arguments
- **Positional Arguments:** Matched by position/order.
- **Keyword Arguments:** Matched by parameter name explicitly.
- **Default Parameters:** Fallback values if arguments are omitted.
  - *Rule:* Non-default parameters must come **before** default parameters.

### 3. Variable Scope (LEGB Rule)
- **Local:** Inside current function.
- **Enclosing:** In outer nested function.
- **Global:** At top-level of script/module.
- **Built-in:** Python pre-defined names (`len`, `sum`, etc.).

### 4. Type Hints & Docstrings
- **Type Hints:** Standardized syntax to specify expected input/output types.
- **Docstrings:** Multi-line strings explaining purpose, parameters, return values, and raised exceptions.

### 5. Modules & File I/O
- **Importing Modules:** `import module`, `import module as alias`, `from module import function`.
- **File Modes:**
  - `'r'`: Read (fails if non-existent).
  - `'w'`: Write (truncates or creates new).
  - `'a'`: Append.
- **Context Manager (`with`):** Ensures automatic resource clean-up and closing.

### 6. Exception Handling & Debugging
- **`try / except / else / finally`:** Catch and handle runtime errors gracefully.
- **`raise`:** Manually trigger exceptions for invalid inputs.
- **`assert`:** Evaluate boolean expressions during execution for internal debugging.
