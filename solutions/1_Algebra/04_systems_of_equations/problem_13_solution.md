# Exercise 13. Does Every Equation Add New Information?

## Problem Statement

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Apply $R_3 \leftarrow R_3 - R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}
$$

Apply $R_3 \leftarrow R_3 + R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Row 3 reduces to $0=0$.

### Part 2. Redundancy Proof

Subtracting equation 2 from equation 1:

$$
(x_1 + x_2) - (x_2 + x_3) = 10 - 8 \implies x_1 - x_3 = 2
$$

Equation 3 is a direct linear combination of equations 1 and 2, providing no independent constraint.

### Part 3. Parametric Solution

Setting $x_3 = t$:

$$
\begin{pmatrix}
x_1 \\
x_2 \\
x_3 \\
\end{pmatrix}=
\begin{pmatrix}
2+t \\
8-t \\
t \\
\end{pmatrix},\qquad t \in \mathbb{R}
$$
