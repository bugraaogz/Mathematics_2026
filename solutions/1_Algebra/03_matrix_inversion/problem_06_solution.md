# Exercise 6. Solving a System Using the Inverse

## Problem Statement

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

---

## Solution

### Part 1. Finding $A^{-1}$

Computing $\det A$:

$$
\det A = 2(3) - 1(1) = 6 - 1 = 5
$$

Using the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

### Part 2. Computing $x = A^{-1}b$

$$
x=A^{-1}b=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=\frac{1}{5}
\begin{pmatrix}
3(5)-1(7) \\
-1(5)+2(7) \\
\end{pmatrix}=\frac{1}{5}
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### Part 3. Verification by Substitution

Substituting $x$ back into $Ax$:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}=
\begin{pmatrix}
2\left(\frac{8}{5}\right) + 1\left(\frac{9}{5}\right) \\
1\left(\frac{8}{5}\right) + 3\left(\frac{9}{5}\right) \\
\end{pmatrix}=
\begin{pmatrix}
\frac{16+9}{5} \\
\frac{8+27}{5} \\
\end{pmatrix}=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=b
$$

The result matches vector $b$.
