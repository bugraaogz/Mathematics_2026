# Exercise 10. Columns of a Matrix Product

## Problem Statement

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

---

## Solution

### Part 1. Computing $Ab_1$ and $Ab_2$

The columns of $B$ are:

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},\qquad b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
$$

Computing $Ab_1$:

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
1(1) + 2(-1) + 0(3) \\
0(1) + 1(-1) + 1(3) \\
\end{pmatrix}=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

Computing $Ab_2$:

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
1(2) + 2(0) + 0(1) \\
0(2) + 1(0) + 1(1) \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

### Part 2. Computing Full Matrix Product $AB$

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1(1)+2(-1)+0(3) & 1(2)+2(0)+0(1) \\
0(1)+1(-1)+1(3) & 0(2)+1(0)+1(1) \\
\end{pmatrix}=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

### Part 3. Comparison and Explanation

Comparing the column-by-column results with $AB$:

$$
AB=
\begin{pmatrix}
Ab_1 & Ab_2 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

Matrix multiplication definition operates such that the $j^{\mathrm{th}}$ column of $AB$ is formed by multiplying matrix $A$ by the $j^{\mathrm{th}}$ column vector $b_j$ of matrix $B$.
