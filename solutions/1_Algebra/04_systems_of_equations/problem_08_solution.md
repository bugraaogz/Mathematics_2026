# Exercise 8. Two Systems with the Same Coefficient Matrix

## Problem Statement

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

---

## Solution

### Part 1. Solving System 1

Augmented matrix $[A \mid b_1]$:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

Swap $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

Back-substitution: $3y = 3 \implies y = 1$; $x - 1 = 1 \implies x = 2$.
Solution 1: $(x,y) = (2,1)$.

### Part 2. Solving System 2

Augmented matrix $[A \mid b_2]$:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$

Swap $R_1$ and $R_2$:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

Back-substitution: $3y = -7 \implies y = -\frac{7}{3}$; $x - \left(-\frac{7}{3}\right) = 4 \implies x = \frac{5}{3}$.
Solution 2: $(x,y) = \left(\frac{5}{3}, -\frac{7}{3}\right)$.

### Part 3. Comparison

The row operations ($R_1 \leftrightarrow R_2$ and $R_2 \leftarrow R_2 - 2R_1$) performed on left side coefficient matrix $A$ are identical in both problems because coefficient matrix $A$ is identical. Only arithmetic operations on right-hand side entries differ.
