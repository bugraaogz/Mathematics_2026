# Exercise 8. Linear Combination and Checking the Result

## Problem Statement

Check whether $w=(5,1)$ can be written as

$$
w=au+bv,
$$

where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$ from them, and explain the geometric meaning of the existence of such coefficients.

---

## Solution

### Part 1. System of Equations

$$
a \begin{pmatrix} 1 \\ 1 \end{pmatrix} + b \begin{pmatrix} 2 \\ -1 \end{pmatrix} = \begin{pmatrix} 5 \\ 1 \end{pmatrix} \implies \begin{cases} a + 2b = 5, \\ a - b = 1. \end{cases}
$$

Subtracting second equation from first:

$$
3b = 4 \implies b = \frac{4}{3}
$$

Substituting $b = \frac{4}{3}$ into $a = 1 + b$:

$$
a = 1 + \frac{4}{3} = \frac{7}{3}
$$

### Part 2. Reconstruction

$$
au + bv = \frac{7}{3}\begin{pmatrix} 1 \\ 1 \end{pmatrix} + \frac{4}{3}\begin{pmatrix} 2 \\ -1 \end{pmatrix} = \begin{pmatrix} \frac{7}{3} + \frac{8}{3} \\ \frac{7}{3} - \frac{4}{3} \end{pmatrix} = \begin{pmatrix} 5 \\ 1 \end{pmatrix} = w
$$

### Part 3. Geometric Meaning

Since $u$ and $v$ are non-parallel vectors in 2D space, they form a basis for $\mathbb{R}^2$. Any vector $w \in \mathbb{R}^2$ can be uniquely decomposed as a linear combination of these basis vectors.
