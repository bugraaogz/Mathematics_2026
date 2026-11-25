# Exercise 7. Choosing a Method Deliberately

## Problem Statement

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

---

## Solution

### Case 1. Triangular System

- **Selected Method:** Direct Back-Substitution.
- **Justification:** Matrix is already upper triangular, so elimination is unnecessary.

**Complete Execution:**
1. From equation 2: $4y = 8 \implies y = 2$.
2. Substitute $y=2$ into equation 1: $2x - 2 = 3 \implies 2x = 5 \implies x = \frac{5}{2}$.

Solution vector:

$$
\begin{pmatrix}
x \\
y \\
\end{pmatrix}=
\begin{pmatrix}
\frac{5}{2} \\
2 \\
\end{pmatrix}
$$

### Case 2. Three Systems with Same Matrix $A$ and Known $A^{-1}$

- **Selected Method:** Matrix Multiplication $x_i = A^{-1} b_i$.
- **Plan & Reusability:** Multiply pre-calculated matrix $A^{-1}$ separately by vectors $b_1, b_2, b_3$.
- **Efficiency:** Known $A^{-1}$ is reused 3 times without repeating elimination steps. Performing full Gaussian elimination 3 times is redundant.

### Case 3. Single $3 \times 3$ System without Given $A^{-1}$

- **Selected Method:** Gaussian Elimination on $[A \mid b]$.
- **Plan & Reusability:** Reduce $[A \mid b]$ to row echelon form and back-substitute.
- **Efficiency:** Computing inverse matrix $A^{-1}$ requires operations on $3 \times 6$ augmented matrix $[A \mid I]$, whereas elimination on $[A \mid b]$ operates on $3 \times 4$ matrix, saving computation steps.
