# Exercise 5. Matrix Times Vector

## Problem Statement

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution

### Part 1. Standard Matrix-Vector Product Computation

$$
Ax=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}=
\begin{pmatrix}
2(4) + (-1)(2) \\
1(4) + 3(2) \\
\end{pmatrix}=
\begin{pmatrix}
8 - 2 \\
4 + 6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

### Part 2. Linear Combination of Columns

The columns of $A$ are:

$$
c_1=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},\qquad c_2=
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

The entries of $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$ serve as scalar coefficients:

$$
Ax = 4 c_1 + 2 c_2 = 4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix} + 2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

This verifies that multiplying a matrix by a vector produces a linear combination of the columns of the matrix weighted by the entries of the vector.
