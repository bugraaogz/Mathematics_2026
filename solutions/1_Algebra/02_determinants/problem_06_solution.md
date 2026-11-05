# Exercise 6. Parameter and Invertibility

## Problem Statement

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

---

## Solution

### Part 1. Computation of Determinant

$$
\det A(t) = t(t) - 1(2) = t^2 - 2
$$

### Part 2. Non-Invertibility Condition

A matrix $A(t)$ is not invertible (singular) if and only if its determinant equals zero:

$$
\det A(t) = 0 \implies t^2 - 2 = 0 \implies t^2 = 2
$$

Solving for $t$:

$$
t = \sqrt{2} \quad \mathrm{or} \quad t = -\sqrt{2}
$$

### Part 3. Explanation

When $t = \pm\sqrt{2}$, the rows of matrix $A(t)$ become linearly dependent. A zero determinant indicates that the matrix maps 2D space onto a 1D subspace (a line), rendering the matrix transformation non-invertible.
