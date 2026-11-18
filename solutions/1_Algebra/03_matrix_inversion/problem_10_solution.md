# Exercise 10. Inverse of a Diagonal Matrix

## Problem Statement

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

---

## Solution

### Part 1. Invertibility Decision

- A diagonal matrix is invertible if and only if all of its diagonal elements are non-zero.
- Matrix $D$ has diagonal entries $2, -3, 5$ (all non-zero, $\det D = -30 \neq 0$), so $D$ is **invertible**.
- Matrix $E$ has a zero entry on its diagonal ($e_{22} = 0$, $\det E = 0$), so $E$ is **singular (not invertible)**.

### Part 2. Finding $D^{-1}$

For a non-singular diagonal matrix, the inverse is obtained by replacing each diagonal entry $d_{ii}$ with $\frac{1}{d_{ii}}$:

$$
D^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}
$$

### Part 3. Verification by Multiplication

$$
DD^{-1}=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}=
\begin{pmatrix}
2\left(\frac{1}{2}\right) & 0 & 0 \\
0 & -3\left(-\frac{1}{3}\right) & 0 \\
0 & 0 & 5\left(\frac{1}{5}\right) \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
$$
