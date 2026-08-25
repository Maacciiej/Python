# Python Lab & Algorithm Implementations

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-Academic-lightgrey.svg)]()
[![Code Style](https://img.shields.io/badge/Code%20Style-PEP8-informational.svg)]()
[![Tests](https://img.shields.io/badge/Tests-unittest-green.svg)]()

A comprehensive collection of Python programming tasks, algorithms, data structures, and standard library utilities developed for academic coursework by **Maciej Filipiak**.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Repository Structure](#-repository-structure)
- [Implemented Modules & Features](#-implemented-modules--features)
  - [1. File System Operations (`os`)](#1-file-system-operations-os)
  - [2. Text Processing & Regular Expressions (`re`)](#2-text-processing--regular-expressions-re)
  - [3. Sorting Algorithms & Verification](#3-sorting-algorithms--verification)
  - [4. Weighted Tree Data Structure (DFS)](#4-weighted-tree-data-structure-dfs)
  - [5. Automated Unit Testing (`unittest`)](#5-automated-unit-testing-unittest)
- [Future & Advanced Exercises](#-future--advanced-exercises)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation & Setup](#installation--setup)
  - [Execution & Running Tests](#execution--running-tests)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 📖 Overview

This repository contains practical implementations exploring core Python features, standard library modules (`os`, `re`, `random`, `unittest`), object-oriented programming, data structures, and algorithm analysis.

Key areas covered:
- Standard I/O and file system manipulation.
- Advanced string substitution and regex pattern matching.
- Implementation and validation of fundamental sorting algorithms.
- Custom hierarchical multi-way tree structure with edge weights.
- Test-Driven Development (TDD) via the `unittest` framework.

---

## 📂 Repository Structure

```plaintext
Python/
│
├── lab01.py        # Complete laboratory script containing all modules, classes, and tests
└── README.md       # Repository documentation and guide
```

---

## ⚙️ Implemented Modules & Features

### 1. File System Operations (`os`)
- **File Counter (`policz_pliki`)**: Inspects a specified target directory using `os.listdir` and `os.path.isfile`, counting all standard files while handling `FileNotFoundError` safely.
- **Recursive Directory Walker (`wypisz_pliki`)**: Traverses arbitrary directory hierarchies recursively via `os.walk`, printing the full paths of all discovered files.

### 2. Text Processing & Regular Expressions (`re`)
- **Word Removal (`usun_slowa_re`)**: Uses dynamically constructed regular expression patterns (`\b` word boundaries and `re.escape`) to cleanly strip targeted words from input text.
- **Dictionary-based Word Replacement (`zamien_slowa_re`)**: Performs multi-word dictionary mappings in a single regex pass utilizing callback functions (`lambda m: mapping[m.group(0)]`).

### 3. Sorting Algorithms & Verification
- **Random Dataset Generator (`generuj_liczby`)**: Generates lists of pseudo-random integers within a specified range using `random.randint`.
- **Bubble Sort (`bubble_sort`)**: Classic $O(n^2)$ comparison-based bubble sort implementation.
- **Insertion Sort (`insertion_sort`)**: In-place $O(n^2)$ insertion sort building the sorted array one element at a time.
- **Automated Validation**: Verifies custom sorting results directly against Python's optimized Timsort (`sorted()`).

### 4. Weighted Tree Data Structure (DFS)
- **`Node` Class**: Represents an individual tree node storing:
  - `value`: Data payload.
  - `children`: List of `(child_node, edge_weight)` tuples.
  - `__str__`: Formatted ASCII hierarchical tree renderer.
  - `traverse()`: Depth-First Search (DFS) traversal returning node values in preorder.
- **`Tree` Class**: Encapsulates the root node and provides high-level traversal and visualization interfaces.

### 5. Automated Unit Testing (`unittest`)
- **`TestTree` Test Suite**:
  - Validates root node initialization.
  - Verifies child counts at multiple tree depths.
  - Checks preorder DFS traversal output consistency.
  - Asserts ASCII hierarchy string formatting.
  - Ensures edge weight integrity.

---

## 🚀 Future & Advanced Exercises

The repository roadmap includes the following upcoming exercises:
1. **Complex Numbers Class**: OOP implementation of complex numbers with operator overloading for addition (`+`) and subtraction (`-`).
2. **Parallel Sorting**: Parallel sorting implementation leveraging Python's `multiprocessing` library.
3. **Performance Benchmarking & Visualization**: Benchmark comparison of serial vs parallel sorting across varying dataset sizes, plotted using `matplotlib`.
4. **Fibonacci Custom Iterator**: Custom iterator class implementing `__iter__` and `__next__` with step control and `StopIteration` handling.

---

## 🛠️ Getting Started

### Prerequisites

- **Python 3.8+** installed on your system.

Verify your installation:
```bash
python --version
# or
python3 --version
```

### Installation & Setup

Clone the repository:
```bash
git clone https://github.com/Maacciiej/Python.git
cd Python
```

### Execution & Running Tests

To run the interactive scripts and unit tests in [`lab01.py`](lab01.py):

```bash
python lab01.py
```

To execute the test suite directly via `unittest`:
```bash
python -m unittest lab01.py
```

---

## 👤 Author & Acknowledgments

- **Author**: Maciej Filipiak ([GitHub: @Maacciiej](https://github.com/Maacciiej))
- **Affiliation**: AGH University of Krakow (AGH UST)
