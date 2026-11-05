# Exercise 1. Determinant of a 2×2 Matrix

## Problem Statement

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},\qquad \det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$

Which matrix is invertible? Justify your answer.

---

## Solution

### Part 1. Computations

For a $2 \times 2$ matrix $\begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the determinant is calculated as $ad - bc$.

First determinant:

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix} = 3(4) - (-2)(5) = 12 + 10 = 22
$$

Second determinant:

$$
\det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix} = 1(14) - 7(2) = 14 - 14 = 0
$$

### Part 2. Invertibility Analysis

A square matrix is invertible if and only if its determinant is non-zero ($\det \neq 0$).

- The first matrix has $\det = 22 \neq 0$, so it is invertible.
- The second matrix has $\det = 0$, so it is singular (not invertible).
