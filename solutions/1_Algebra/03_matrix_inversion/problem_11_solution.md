# Exercise 11. Parameter and Invertibility

## Problem Statement

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

---

## Solution

### Part 1. Invertibility Condition

Computing the determinant:

$$
\det A(t) = 1(1) - t(t) = 1 - t^2
$$

Matrix $A(t)$ is invertible if and only if $\det A(t) \neq 0$:

$$
1 - t^2 \neq 0 \implies t^2 \neq 1 \implies t \neq 1 \quad \mathrm{and} \quad t \neq -1
$$

### Part 2. Formula for $A(t)^{-1}$

Using the $2 \times 2$ matrix inverse formula for $t \neq \pm 1$:

$$
A(t)^{-1} = \frac{1}{1 - t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{1 - t^2} & \frac{-t}{1 - t^2} \\
\frac{-t}{1 - t^2} & \frac{1}{1 - t^2} \\
\end{pmatrix}
$$

### Part 3. Explanation of Excluded Values

At $t = 1$ or $t = -1$, the denominator $1 - t^2$ becomes zero, rendering the formula undefined. At these values, the rows of $A(t)$ become identical ($t=1$) or opposites ($t=-1$), collapsing 2D space into 1D space.
