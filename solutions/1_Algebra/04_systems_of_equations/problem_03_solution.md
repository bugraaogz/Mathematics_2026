# Exercise 3. Inconsistent System

## Problem Statement

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

Apply operation $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

### Part 2. Matrix and Equation Interpretation

The second row corresponds to equation:

$$
0x + 0y = 1 \implies 0 = 1
$$

This equation creates an absolute contradiction ($0 = 1$).

### Part 3. Geometric and Algebraic Conclusion

Geometrically, the equations $x+2y=3$ and $2x+4y=7$ represent two parallel lines with identical slope ($m = -\frac{1}{2}$) but different $y$-intercepts. The lines never intersect, so the system is **inconsistent** and has **no solution**.
