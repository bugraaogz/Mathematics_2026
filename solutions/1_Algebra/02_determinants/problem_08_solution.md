# Exercise 8. Determinant of a Product

## Problem Statement

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

---

## Solution

### Part 1. Computations

#### Computation of $\det(AB)$

Using the multiplicative property of determinants:

$$
\det(AB) = \det A \cdot \det B = 3 \cdot (-5) = -15
$$

#### Computation of $\det(BA)$

$$
\det(BA) = \det B \cdot \det A = (-5) \cdot 3 = -15
$$

#### Computation of $\det(A^{-1}B)$

Since $\det A = 3 \neq 0$, $A^{-1}$ exists and $\det(A^{-1}) = \frac{1}{\det A}$:

$$
\det(A^{-1}B) = \det(A^{-1}) \cdot \det B = \frac{1}{3} \cdot (-5) = -\frac{5}{3}
$$

### Part 2. Explanation of $\det(AB) = \det(BA)$

Although matrix multiplication is non-commutative ($AB \neq BA$), the determinants $\det A$ and $\det B$ are real numbers (scalars). Because multiplication of real numbers is commutative:

$$
\det A \cdot \det B = \det B \cdot \det A \implies \det(AB) = \det(BA) = -15
$$
