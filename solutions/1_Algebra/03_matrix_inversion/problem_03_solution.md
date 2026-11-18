# Exercise 3. When Does the Inverse Not Exist?

## Problem Statement

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

---

## Solution

### Method 1. Using the Determinant

A matrix $A$ is invertible if and only if $\det A \neq 0$.

Computing $\det A$:

$$
\det A = 2(2) - 4(1) = 4 - 4 = 0
$$

Since $\det A = 0$, matrix $A$ is singular and its inverse $A^{-1}$ does not exist.

### Method 2. Using Row Dependence

Examining the rows of matrix $A$:

$$
R_1 =
\begin{pmatrix}
2 & 4 \\
\end{pmatrix},\qquad R_2 =
\begin{pmatrix}
1 & 2 \\
\end{pmatrix}
$$

Notice that $R_1 = 2 R_2$. The rows are linearly dependent, which means the matrix maps 2D space onto a 1D line. Information is lost during this transformation, making it impossible to undo. Thus, $A^{-1}$ does not exist.
