# Exercise 2. Formula for a 2×2 Matrix

## Problem Statement

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

---

## Solution

### Part 1. Finding the Inverse

For a general $2 \times 2$ matrix $\begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the inverse formula is:

$$
A^{-1} = \frac{1}{\det A}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}
$$

First compute $\det A$:

$$
\det A = 3(4) - 2(5) = 12 - 10 = 2
$$

Applying the formula:

$$
A^{-1} = \frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}
$$

### Part 2. Verification by Multiplication

Computing $A A^{-1}$:

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}=
\begin{pmatrix}
3(2)+2\left(-\frac{5}{2}\right) & 3(-1)+2\left(\frac{3}{2}\right) \\
5(2)+4\left(-\frac{5}{2}\right) & 5(-1)+4\left(\frac{3}{2}\right) \\
\end{pmatrix}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

The multiplication yields the identity matrix, verifying the result.
