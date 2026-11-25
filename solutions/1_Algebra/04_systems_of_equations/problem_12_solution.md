# Exercise 12. Homogeneous System

## Problem Statement

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid 0]$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

Interchange $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### Part 2. Parametric Solution

From row 2: $-3y + 3z = 0 \implies y = z$.
From row 1: $x + 2z - z = 0 \implies x = -z$.

Set $z = t$ ($t \in \mathbb{R}$):

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
-t \\
t \\
t \\
\end{pmatrix}
$$

### Part 3. Trivial Solution Explanation

For any homogeneous linear system $Ax = 0$, substituting zero vector $x = 0$ yields $A \cdot 0 = 0$. Matrix multiplication of any matrix by zero vector always results in zero vector, making $(0,0,0)$ a universal solution (trivial solution).
