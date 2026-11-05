# Exercise 9. Area and the Determinant

## Problem Statement

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},\qquad v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

---

## Solution

### Part 1. Area Computation

Form a matrix $M$ using $u$ and $v$ as columns:

$$
M=
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
$$

Computing the determinant:

$$
\det M = 3(4) - 1(1) = 12 - 1 = 11
$$

The area of the parallelogram is given by the absolute value of the determinant:

$$
\mathrm{Area} = |\det M| = |11| = 11
$$

### Part 2. Reversing Vector Order

Reversing vector order yields matrix $M'$:

$$
M'=
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
$$

Computing the new determinant:

$$
\det M' = 1(1) - 3(4) = 1 - 12 = -11
$$

### Part 3. Explanation

- **What changes:** The determinant changes sign from $+11$ to $-11$ because swapping two columns reverses orientation (from counterclockwise to clockwise).
- **What stays the same:** The geometric area remains unchanged because area is non-negative: $\mathrm{Area} = |-11| = 11$.
