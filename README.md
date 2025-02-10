# s21_containers - Custom Container Library

## Contents
1. [Introduction](#introduction)
2. [Container Information](#container-information)
3. [Library Implementation](#library-implementation)
   1. [Part 1: Basic Containers](#part-1-basic-containers)
   2. [Part 2: Bonus Containers](#part-2-bonus-containers)
   3. [Part 3: Bonus - `insert_many`](#part-3-bonus--insert_many)

## Introduction

The project involves implementing custom C++ containers: `list`, `map`, `queue`, `set`, `stack`, and `vector`. These containers should mimic the Standard Template Library (STL) with support for basic methods like element access, iteration, capacity checking, and element manipulation. Bonus tasks involve adding additional containers like `array` and `multiset`, and implementing the `insert_many` method.

## Container Information

Containers hold collections of objects, where each type of container (like lists, sets, or maps) offers unique organization and interaction methods. Containers are template classes to handle various data types. The containers must also support iterators, which are similar to pointers for traversing elements.

**Iterator operations include:**
- Accessing elements (`*iter`)
- Moving iterators forward (`++iter`) and backward (`--iter`)
- Comparison (`iter1 == iter2`, `iter1 != iter2`)

## Library Implementation

- **C++17** standards, using GCC compiler.
- The containers must be implemented as template classes in the `s21` namespace.
- Full unit test coverage using the GTest library is required.
- The STL logic must be followed (e.g., memory handling, abnormal situation checks).

### Part 1: Basic Containers
You need to implement:
- `list`, `map`, `queue`, `set`, `stack`, `vector`
- Provide a header file (`s21_containers.h`) that includes all implementations.
- Use iterators for element access and provide standard methods for each container (add, remove, check capacity, etc.).

### Part 2: Bonus - Additional Containers
Implement additional containers:
- `array`, `multiset`
- Implement the containers in a new header file (`s21_containersplus.h`).

### Part 3: Bonus - `insert_many` Method
Implement the `insert_many` method for containers like `list`, `vector`, `queue`, `stack`, `map`, `set`, and `multiset`. This method should allow inserting multiple elements at once using a parameter pack (`Args&&... args`).

**Examples of `insert_many` variants:**
- Insert elements before a specific iterator: `iterator insert_many(const_iterator pos, Args&&... args)`
- Insert elements at the end or front of containers like `list`, `vector`, `stack`, etc.

## Conclusion
This project will help you learn how to implement custom container classes with a deep understanding of C++ templating, memory management, and iterator operations.
