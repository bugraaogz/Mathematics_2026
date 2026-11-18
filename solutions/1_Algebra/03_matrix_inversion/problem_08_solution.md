# Exercise 8. Inverse of a Transformation

## Problem Statement

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

---

## Solution

### Part 1. Finding $S^{-1}$

For a diagonal matrix, the inverse is formed by taking the reciprocal of each diagonal entry:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
$$

### Part 2. Geometric Interpretation

- Transformation $S$ stretches the $x$-axis by a factor of $2$ and compresses the $y$-axis by a factor of $\frac{1}{2}$.
- The inverse transformation $S^{-1}$ undoes this action by compressing the $x$-axis by a factor of $\frac{1}{2}$ and stretching the $y$-axis by a factor of $2$.

### Part 3. Verification on a Vector

Choose vector $v = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$.

Applying $S$ to $v$:

$$
Sv=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}=
\begin{pmatrix}
8 \\
1 \\
\end{pmatrix}
$$

Now applying $S^{-1}$ to $Sv$:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
8 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}=v
$$

The original vector $v$ is restored.
