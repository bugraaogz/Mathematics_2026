# Exercise 12. Finding Inverses Without Starting from Scratch

## Problem Statement

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

---

## Solution

### 1. Computation of $(3A)^{-1}$

**Property:** $(cA)^{-1} = c^{-1} A^{-1} = \frac{1}{c} A^{-1}$ for non-zero scalar $c$.

$$
(3A)^{-1} = \frac{1}{3} A^{-1} = \frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3} \\
\end{pmatrix}
$$

### 2. Computation of $(A^T)^{-1}$

**Property:** $(A^T)^{-1} = (A^{-1})^T$. Transposition and inversion commute.

$$
(A^T)^{-1} = (A^{-1})^T =
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}
$$

### 3. Computation of $(A^2)^{-1}$

**Property:** $(A^2)^{-1} = (A^{-1})^2$.

$$
(A^2)^{-1} = (A^{-1})^2 =
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2(2)+(-1)(-3) & 2(-1)+(-1)(2) \\
-3(2)+2(-3) & -3(-1)+2(2) \\
\end{pmatrix}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}
$$
