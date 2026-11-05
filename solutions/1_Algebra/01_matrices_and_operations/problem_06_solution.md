# Exercise 6. Transpose

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

---

## Solution

### Part 1. Computing Transposes

The transpose of a matrix is formed by swapping its rows and columns.

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

$$
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

### Part 2. Computing $AB$ and $(AB)^T$

$$
AB=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
1(1)+2(2)+3(-1) & 1(0)+2(1)+3(3) \\
4(1)+5(2)+6(-1) & 4(0)+5(1)+6(3) \\
\end{pmatrix}=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

Taking the transpose of $AB$:

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

### Part 3. Computing $B^TA^T$ and Verification

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}=
\begin{pmatrix}
1(1)+2(2)+(-1)(3) & 1(4)+2(5)+(-1)(6) \\
0(1)+1(2)+3(3) & 0(4)+1(5)+3(6) \\
\end{pmatrix}=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

Both sides yield the identical matrix:

$$
(AB)^T = B^TA^T =
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

This verifies the transpose-of-a-product identity $(AB)^T = B^TA^T$.
