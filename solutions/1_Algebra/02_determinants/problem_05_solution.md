# Exercise 5. Row Operations

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

---

## Solution

### Step-by-Step Row Reduction

1. Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 + R_1$:
   - **Effect on determinant:** Adding a scalar multiple of one row to another row does not change the determinant.

$$
A_1=
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix},\qquad \det A = \det A_1
$$

2. Apply $R_3 \leftarrow R_3 + 2R_2$:
   - **Effect on determinant:** Adding a scalar multiple of one row to another row does not change the determinant.

$$
A_2=
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix},\qquad \det A = \det A_2
$$

### Final Determinant Calculation

Matrix $A_2$ is in upper triangular form. Its determinant is the product of diagonal entries:

$$
\det A = \det A_2 = 1 \cdot (-3) \cdot (-7) = 21
$$
