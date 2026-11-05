# Exercise 4. Triangular Matrix

## Problem Statement

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

---

## Solution

### Part 1. Calculation

The given matrix is upper triangular (all entries below the main diagonal are zero).

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix} = 2 \cdot (-3) \cdot 7 = -42
$$

### Part 2. General Rule and Explanation

**Rule:** The determinant of a upper or lower triangular matrix is equal to the product of its main diagonal elements.

**Explanation:** Performing cofactor expansion along the first column of an upper triangular matrix:

$$
\det A = a_{11} \cdot \det A_{11} - 0 + 0 = a_{11} (a_{22} a_{33} - 0) = a_{11} a_{22} a_{33}
$$

For this specific matrix, $2 \cdot (-3) \cdot 7 = -42$.
