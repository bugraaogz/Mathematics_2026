# Exercise 2. Gaussian Elimination — One Solution

## Problem Statement

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

1. Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

2. Interchange $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

3. Apply $R_3 \leftarrow R_3 + 3R_2$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

### Part 2. Back-Substitution

From row 3:

$$
-7z = -21 \implies z = 3
$$

From row 2:

$$
y - 2(3) = -4 \implies y = 2
$$

From row 1:

$$
x + 2 + 3 = 6 \implies x = 1
$$

The unique solution vector is:

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
1 \\
2 \\
3 \\
\end{pmatrix}
$$

### Part 3. Verification

Substituting $(1,2,3)$ into original equations:

- Equation 1: $1 + 2 + 3 = 6$
- Equation 2: $2(1) - 2 + 3 = 3$
- Equation 3: $1 + 2(2) - 3 = 2$

All equations are satisfied.
