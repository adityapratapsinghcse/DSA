# ⚡ LeetCode Constraint & Complexity Cheat Sheet

One of the fastest ways to identify the correct approach for a problem is to look at the **Constraints** section before writing any code.

The input size (**N**) often tells you what time complexity is expected.

## 📊 Complexity Guide

| Input Size (N) | Expected Time Complexity | Common Techniques                              |
| -------------- | ------------------------ | ---------------------------------------------- |
| N ≤ 10 - 20    | O(2ⁿ) or O(N!)           | Backtracking, Recursion, Brute Force           |
| N ≤ 100        | O(N³)                    | Triple Nested Loops                            |
| N ≤ 1,000      | O(N²)                    | Double Nested Loops                            |
| N ≤ 10⁵ - 10⁶  | O(N log N) or O(N)       | Sliding Window, Two Pointers, Hashing, Sorting |
| N ≤ 10⁹        | O(log N) or O(1)         | Binary Search, Mathematical Formulas           |

---

## 🧠 Why Constraints Matter

Before solving a problem, always estimate the maximum number of operations your solution may perform.

### Example

If:

```text
N = 100,000
```

and your solution uses:

```text
O(N²)
```

then:

```text
100,000 × 100,000
= 10,000,000,000
= 10¹⁰ operations
```

This is far too slow and will likely result in:

```text
TLE (Time Limit Exceeded)
```

---

## ⚡ Competitive Programming Rule

A modern online judge can generally handle approximately:

| Operations | Usually Acceptable |
| ---------- | ------------------ |
| 10⁶        | Instant            |
| 10⁷        | Very Fast          |
| 10⁸        | Usually Safe       |
| 10⁹        | Risky              |
| 10¹⁰+      | Likely TLE         |

---

## 🎯 Constraint → Pattern Mapping

### N ≤ 20

Think:

* Backtracking
* Recursion
* Generate All Possibilities
* Subsets
* Permutations

Examples:

* N Queens
* Subsets
* Permutations
* Sudoku Solver

---

### N ≤ 1,000

Think:

* Nested Loops
* Dynamic Programming
* Matrix Problems

Examples:

* Longest Increasing Subsequence (O(N²))
* Interval Problems
* DP Basics

---

### N ≤ 100,000

Think:

* Sliding Window
* Two Pointers
* Hash Maps
* Prefix Sum
* Greedy
* Monotonic Stack

Examples:

* Longest Substring Without Repeating Characters
* Two Sum
* Daily Temperatures
* Maximum Subarray

---

### N ≤ 1,000,000

Think:

* Single Pass Solutions
* O(N)
* O(N log N)

Examples:

* Sorting
* Frequency Counting
* Prefix/Suffix Computations

---

### N ≤ 10⁹

Think:

* Binary Search
* Mathematics
* Logarithmic Solutions

Examples:

* Search Space Problems
* Square Root Problems
* Capacity to Ship Packages
* Koko Eating Bananas

---

## 🚨 Interview Tip

Before writing code, ask yourself:

1. What is the maximum input size?
2. What time complexity can pass?
3. Which algorithmic pattern fits that complexity?

Many LeetCode problems become significantly easier once the constraints reveal the expected solution.

---

## 💡 Golden Rule

**Constraints often reveal the solution pattern before the problem statement does.**

Always read the constraints first.
