# 0x02. Minimum Operations

This repository contains a solution to the problem of calculating the minimum number of operations needed to achieve a given number of characters using only "Copy All" and "Paste" operations.

## Description

In a text file, there is a single character `H`. Your text editor can execute only two operations in this file: Copy All and Paste. Given a number `n`, write a method that calculates the fewest number of operations needed to result in exactly `n` `H` characters in the file.

## Concepts Needed

To devise an efficient solution for this problem, it is helpful to understand the following concepts:

1. **Dynamic Programming**:
   - Breaking down the problem into simpler subproblems and building up the solution.
   - [Dynamic Programming (GeeksforGeeks)](https://www.geeksforgeeks.org/dynamic-programming/)

2. **Prime Factorization**:
   - Understanding prime factorization is crucial since the problem can be reduced to finding the sum of the prime factors of the target number `n`.
   - [Prime Factorization (Khan Academy)](https://www.khanacademy.org/math/algebra/x15aaf8a5d3bb4ae7:polynomials/x15aaf8a5d3bb4ae7:factoring-polynomials/a/intro-to-polynomial-factorization-review)

3. **Code Optimization**:
   - Approaching problems from an optimization perspective to find the most efficient solution.
   - [How to optimize Python code](https://realpython.com/python-performance/)

4. **Greedy Algorithms**:
   - Choosing the best option at each step.
   - [Greedy Algorithms (GeeksforGeeks)](https://www.geeksforgeeks.org/greedy-algorithms/)

5. **Basic Python Programming**:
   - Proficiency in Python, including loops, conditionals, and functions, is necessary to implement the solution.
   - [Python Functions (Python Official Documentation)](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All your files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should be documented
- Your code should use the PEP 8 style (version 1.7.x)
- All your files must be executable

## Tasks

### Task 0: Minimum Operations

- **File**: `0-minoperations.py`
- **Description**: Write a method that calculates the fewest number of operations needed to result in exactly `n` `H` characters in the file.
- **Prototype**: `def minOperations(n)`
- **Returns**: An integer, the minimum number of operations needed. If `n` is impossible to achieve, return `0`.

#### Example

```python
n = 9

H => Copy All => Paste => HH => Paste =>HHH => Copy All => Paste => HHHHHH => Paste => HHHHHHHHH

Number of operations: 6
