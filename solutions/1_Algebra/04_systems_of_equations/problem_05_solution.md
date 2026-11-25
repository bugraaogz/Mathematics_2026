# Exercise 5. Row Echelon Form and Number of Solutions

## Problem Statement

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

---

## Solution

### Part 1. Free Variables Determination

Let variables be $x_1, x_2, x_3$.
- Pivot elements are located in column 1 ($x_1$) and column 2 ($x_2$).
- Matrix rank is $\mathrm{rank}(A) = 2$ and augmented matrix rank is $\mathrm{rank}([A \mid b]) = 2$.
- Number of unknowns is $n = 3$.

Number of free variables equals $n - \mathrm{rank}(A) = 3 - 2 = 1$. Column 3 contains no pivot, so variable $x_3$ is chosen freely ($x_3 = t$, where $t \in \mathbb{R}$).

### Part 2. Parametric Solution Construction

From row 2:

$$
x_2 + 2t = 1 \implies x_2 = 1 - 2t
$$

From row 1:

$$
x_1 + 2(1 - 2t) - t = 3 \implies x_1 + 2 - 5t = 3 \implies x_1 = 1 + 5t
$$

Parametric solution:

$$
\begin{pmatrix}
x_1 \\
x_2 \\
x_3 \\
\end{pmatrix}=
\begin{pmatrix}
1+5t \\
1-2t \\
t \\
\end{pmatrix},\qquad t \in \mathbb{R}
$$

### Part 3. Conclusion

Because there is one free variable parameterizing the solution set, the system has **infinitely many solutions**.
