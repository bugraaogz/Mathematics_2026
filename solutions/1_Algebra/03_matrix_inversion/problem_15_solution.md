# Exercise 15. Two Methods for Solving the Same System

## Problem Statement

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

---

## Solution

### Method 1. Using Matrix Inverse $x = A^{-1}b$

1. Compute $\det A = 2(3) - 1(1) = 5$.
2. Compute $A^{-1} = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}$.
3. Multiply $A^{-1}b$:

$$
x=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}=\frac{1}{5}
\begin{pmatrix}
3(7)-1(8) \\
-1(7)+2(8) \\
\end{pmatrix}=\frac{1}{5}
\begin{pmatrix}
13 \\
9 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### Method 2. Using Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

1. Interchange $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

2. Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

3. Back-substitution:
   - Second row gives $-5y = -9 \implies y = \frac{9}{5}$.
   - First row gives $x + 3y = 8 \implies x = 8 - 3\left(\frac{9}{5}\right) = \frac{40-27}{5} = \frac{13}{5}$.

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### Comparison and Method Selection

- Both methods give the exact same solution vector $x = \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix}$.
- **Gaussian elimination** requires fewer arithmetic operations because it avoids calculating all entries of the inverse matrix explicitly. Thus, Gaussian elimination is simpler for solving a single linear system.
