# Exercise 3. Swapping Two Rows

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

---

## Solution

### Part 1. Computation of $\det A$

Expanding along the first row:

$$
\det A = 1 \cdot \det
\begin{pmatrix}
3 & 1 \\
1 & 1 \\
\end{pmatrix} - 2 \cdot \det
\begin{pmatrix}
0 & 1 \\
2 & 1 \\
\end{pmatrix} + 0
$$

$$
\det A = 1(3 - 1) - 2(0 - 2) = 2 - 2(-2) = 2 + 4 = 6
$$

### Part 2. Prediction of $\det B$

Matrix $B$ is formed by swapping row 1 and row 2 of matrix $A$:

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

**Property:** Swapping two rows of a square matrix changes the sign of its determinant.
Therefore, we predict:

$$
\det B = -\det A = -6
$$

### Part 3. Verification by Direct Calculation

Expanding along the first row of $B$:

$$
\det B = 0 - 3 \cdot \det
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
\end{pmatrix} + 1 \cdot \det
\begin{pmatrix}
1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

$$
\det B = 0 - 3(1 - 0) + 1(1 - 4) = -3 + (-3) = -6
$$

The calculation confirms the prediction.
