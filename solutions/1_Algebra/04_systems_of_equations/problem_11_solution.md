# Exercise 11. A Parameter in a System of Three Equations

## Problem Statement

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

### Part 2. Parameter Analysis

1. **Excluded Case $t = 1$:**
   For $t=1$, row 2 becomes $\begin{pmatrix} 0 & 0 & 0 & \mid & 1 \end{pmatrix}$, giving equation $0 = 1$. The system is inconsistent and has **no solution**.

2. **Standard Case $t \neq 1$:**
   Row 2 gives $(t-1)y = 1 \implies y = \frac{1}{t-1}$.
   Row 3 gives $(t-1)z = 2 \implies z = \frac{2}{t-1}$.
   Row 1 gives:

$$
x = 1 - y - z = 1 - \frac{1}{t-1} - \frac{2}{t-1} = 1 - \frac{3}{t-1} = \frac{t-4}{t-1}
$$

For $t \neq 1$, system has **exactly one solution**:

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
\frac{t-4}{t-1} \\
\frac{1}{t-1} \\
\frac{2}{t-1} \\
\end{pmatrix}
$$

Infinitely many solutions case does not occur for any value of $t$.
