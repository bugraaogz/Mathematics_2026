# Exercise 2. Determinant of a 3×3 Matrix

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

---

## Solution

### Part 1. Computation using Sarrus' Rule

According to Sarrus' rule for a $3 \times 3$ matrix:

$$
\det A = (a_{11}a_{22}a_{33} + a_{12}a_{23}a_{31} + a_{13}a_{21}a_{32}) - (a_{13}a_{22}a_{31} + a_{11}a_{23}a_{32} + a_{12}a_{21}a_{33})
$$

Positive terms:

$$
1(3)(5) + 2(4)(2) + (-1)(0)(1) = 15 + 16 + 0 = 31
$$

Negative terms:

$$
(-1)(3)(2) + 1(4)(1) + 2(0)(5) = -6 + 4 + 0 = -2
$$

Subtracting negative terms from positive terms:

$$
\det A = 31 - (-2) = 33
$$

### Part 2. Verification using Cofactor Expansion

Expanding along the first column of matrix $A$:

$$
\det A = 1 \cdot \det
\begin{pmatrix}
3 & 4 \\
1 & 5 \\
\end{pmatrix} - 0 \cdot \det
\begin{pmatrix}
2 & -1 \\
1 & 5 \\
\end{pmatrix} + 2 \cdot \det
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$
\det A = 1(15 - 4) - 0 + 2(8 - (-3)) = 1(11) + 2(11) = 11 + 22 = 33
$$

The result matches the Sarrus' rule calculation.
