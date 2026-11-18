# Exercise 7. Inverse of a Product

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

---

## Solution

### Part 1. Computing $(AB)^{-1}$

First compute $AB$:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
$$

$\det(AB) = 2(3) - 3(0) = 6$. Finding $(AB)^{-1}$:

$$
(AB)^{-1}=\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

### Part 2. Computing $B^{-1}A^{-1}$

Inverses of individual matrices:

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

Multiplying $B^{-1}A^{-1}$:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

### Part 3. Comparison and Explanation

Both methods yield the exact same matrix:

$$
(AB)^{-1} = B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}
$$

The reversed order arises because operation $AB$ applies $B$ first, then $A$. To undo this combined process, one must reverse the operations in backward order: undo $A$ first ($A^{-1}$), then undo $B$ ($B^{-1}$).
