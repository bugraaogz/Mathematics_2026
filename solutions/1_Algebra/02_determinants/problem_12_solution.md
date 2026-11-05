# Exercise 12. A Parameter Revealed by a Row Operation

## Problem Statement

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

---

## Solution

### Part 1. Row Operation

Performing $R_2 \leftarrow R_2 - 2R_1$ (which leaves the determinant unchanged):

$$
A_1(t)=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad \det A(t) = \det A_1(t)
$$

### Part 2. Swapping Rows to Form Triangular Matrix

Interchanging $R_2$ and $R_3$ (changes the sign of the determinant):

$$
A_2(t)=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & t-6 \\
\end{pmatrix},\qquad \det A(t) = -\det A_2(t)
$$

The determinant of upper triangular matrix $A_2(t)$ is $1 \cdot 1 \cdot (t-6) = t-6$.
Therefore:

$$
\det A(t) = -(t - 6) = 6 - t
$$

### Part 3. Non-Invertibility and Row Structure

The matrix is not invertible when $\det A(t) = 0$:

$$
6 - t = 0 \implies t = 6
$$

When $t = 6$, the second row of original matrix $A(6)$ becomes $\begin{pmatrix} 2 & 4 & 6 \end{pmatrix}$, which is exactly $2 R_1$. This makes row 1 and row 2 linearly dependent.
