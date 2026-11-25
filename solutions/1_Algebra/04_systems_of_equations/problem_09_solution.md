# Exercise 9. A System from a Sum Condition

## Problem Statement

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

---

## Solution

### Part 1. Algebraic Solution

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}
$$

From row 2: $3y = 12 \implies y = 4$.
From row 1: $x + 4 = 10 \implies x = 6$.

Unique solution: $(x,y) = (6,4)$.

### Part 2. Geometric Explanation

The linear equations describe two lines in $\mathbb{R}^2$:

- Line 1: $y = -x + 10$ (slope $m_1 = -1$)
- Line 2: $y = -\frac{2}{5}x + \frac{32}{5}$ (slope $m_2 = -\frac{2}{5}$)

Because slopes are unequal ($m_1 \neq m_2$), the lines are not parallel and intersect at exactly one unique point $(6,4)$.
