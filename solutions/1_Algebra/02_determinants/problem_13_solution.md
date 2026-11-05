# Exercise 13. Determinant by Elimination

## Problem Statement

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

---

## Solution

### Step 1. $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$

Adding/subtracting scalar multiples of rows leaves the determinant unchanged.

$$
A_1=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix},\qquad \det A = \det A_1
$$

### Step 2. $R_3 \leftarrow R_3 + 2R_2$

Adding twice row 2 to row 3 leaves the determinant unchanged.

$$
A_2=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix},\qquad \det A = \det A_2
$$

### Step 3. Product of Diagonal Entries

Matrix $A_2$ is in upper triangular form:

$$
\det A = 1 \cdot 1 \cdot 1 = 1
$$
