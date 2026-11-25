# Exercise 9. Cross Product as a Perpendicular Direction

## Problem Statement

For $u=(1,2,0)$ and $v=(0,1,3)$ compute $u\times v$. Use dot products to check perpendicularity to both vectors, compute $v\times u$, and compare the results.

---

## Solution

### Part 1. Computation of $u \times v$

$$
u \times v = \det \begin{pmatrix} i & j & k \\ 1 & 2 & 0 \\ 0 & 1 & 3 \end{pmatrix} = i(6 - 0) - j(3 - 0) + k(1 - 0) = \begin{pmatrix} 6 \\ -3 \\ 1 \end{pmatrix}
$$

### Part 2. Perpendicularity Check

$$
(u \times v) \cdot u = 6(1) + (-3)(2) + 1(0) = 6 - 6 + 0 = 0
$$

$$
(u \times v) \cdot v = 6(0) + (-3)(1) + 1(3) = 0 - 3 + 3 = 0
$$

### Part 3. Computation of $v \times u$ and Comparison

$$
v \times u = \det \begin{pmatrix} i & j & k \\ 0 & 1 & 3 \\ 1 & 2 & 0 \end{pmatrix} = i(0 - 6) - j(0 - 3) + k(0 - 1) = \begin{pmatrix} -6 \\ 3 \\ -1 \end{pmatrix}
$$

**Comparison:** $v \times u = -(u \times v)$. Reversing the product order negates the vector, reversing orientation while preserving magnitude.
