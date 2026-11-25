# Exercise 4. Infinitely Many Solutions

## Problem Statement

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

---

## Solution

### Part 1. Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

Interchange $R_2$ and $R_3$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### Part 2. Parametric Solution

From row 2: $-2y = -2 \implies y = 1$.
From row 1: $x + 1 + z = 2 \implies x = 1 - z$.

Set $z$ as the free variable ($z = t$, where $t \in \mathbb{R}$):

$$
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
1-t \\
1 \\
t \\
\end{pmatrix}
$$

The system has infinitely many solutions.

### Part 3. Verification for $t = 0$

Setting parameter $t = 0$ yields point $(x,y,z) = (1,1,0)$:

- Equation 1: $1 + 1 + 0 = 2$
- Equation 2: $2(1) + 2(1) + 2(0) = 4$
- Equation 3: $1 - 1 + 0 = 0$

All equations are satisfied.
