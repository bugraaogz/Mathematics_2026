# Exercise 10. Detecting Dependence

## Problem Statement

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

---

## Solution

### Part 1. Identifying Row Dependence

Let the rows of the matrix be $R_1, R_2, R_3$:

$$
R_1 =
\begin{pmatrix}
1 & 2 & 3 \\
\end{pmatrix},\qquad R_2 =
\begin{pmatrix}
2 & 4 & 6 \\
\end{pmatrix},\qquad R_3 =
\begin{pmatrix}
0 & 1 & 5 \\
\end{pmatrix}
$$

Notice that row 2 is exactly twice row 1:

$$
R_2 = 2 R_1
$$

### Part 2. Reason for Zero Determinant

If one row of a matrix is a scalar multiple of another row, the rows are linearly dependent. Applying the row operation $R_2 \leftarrow R_2 - 2R_1$ produces a row of zeros:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}
$$

Any matrix containing a zero row has determinant equal to $0$.

### Part 3. Connection to Noninvertibility

Linear dependence among rows reduces the rank of the matrix ($\mathrm{rank} < 3$), making the matrix singular (non-invertible).
