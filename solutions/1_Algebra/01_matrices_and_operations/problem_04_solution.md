# Exercise 4. Matrix Multiplication and Noncommutativity

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

---

## Solution

### Part 1. Computations

#### Computing $AB$

$$
AB=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1(2)+2(3) & 1(0)+2(1) \\
0(2)+1(3) & 0(0)+1(1) \\
\end{pmatrix}=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### Computing $BA$

$$
BA=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2(1)+0(0) & 2(2)+0(1) \\
3(1)+1(0) & 3(2)+1(1) \\
\end{pmatrix}=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

### Part 2. Noncommutativity Analysis

Comparing the two resulting matrices:

$$
AB =
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
\neq
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
= BA
$$

Therefore, $AB \neq BA$. 

In ordinary real-number algebra, multiplication is commutative ($ab = ba$). However, matrix multiplication is in general non-commutative. The order of factors matters because rows of the first matrix are paired with columns of the second, and changing the order alters these pairings entirely.
