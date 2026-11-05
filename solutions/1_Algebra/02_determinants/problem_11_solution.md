# Exercise 11. Shortening the Calculation with Row Operations

## Problem Statement

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

---

## Solution

### Part 1. Row Operations

1. Apply $R_2 \leftarrow R_2 - R_1$ and $R_3 \leftarrow R_3 - R_1$:
   - **Property:** Subtracting one row from another does not change the determinant value.

$$
A_1=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix},\qquad \det A = \det A_1
$$

2. Apply $R_3 \leftarrow R_3 - 2R_2$:
   - **Property:** Subtracting a scalar multiple of one row from another does not change the determinant value.

$$
A_2=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix},\qquad \det A = \det A_2
$$

### Part 2. Final Computation

Matrix $A_2$ is in upper triangular form. The determinant is the product of its diagonal elements:

$$
\det A = 1 \cdot 1 \cdot 1 = 1
$$
