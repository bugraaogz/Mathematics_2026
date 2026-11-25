# Exercise 7. Linear Dependence Without Heavy Computation

## Problem Statement

Given

$$
u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1).
$$

Identify a specific relation between $u$ and $v$, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

---

## Solution

### Part 1. Vector Relation

Notice that $v$ is a direct scalar multiple of $u$:

$$
v = 2u
$$

### Part 2. Linear Independence Analysis

The set $\{u, v, w\}$ cannot be linearly independent. Since $v = 2u$, the subset $\{u, v\}$ is linearly dependent ($2u - v + 0w = 0$), making the entire set $\{u, v, w\}$ linearly dependent.

### Part 3. Explanation

No long calculation (such as Gaussian elimination or determinant evaluation) is needed because scalar proportionality between two vectors ($v = 2u$) is immediately visible by inspection.
