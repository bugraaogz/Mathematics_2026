# Exercise 7. Using Properties Instead of Recomputing

## Problem Statement

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

---

## Solution

### 1. Computation of $\det(2A)$

**Property:** For an $n \times n$ matrix, $\det(cA) = c^n \det A$.
Here $n = 3$ and $c = 2$:

$$
\det(2A) = 2^3 \det A = 8 \cdot (-4) = -32
$$

### 2. Computation of $\det(A^T)$

**Property:** Transposition does not change the determinant: $\det(A^T) = \det A$.

$$
\det(A^T) = -4
$$

### 3. Computation of $\det(A^2)$

**Property:** $\det(AB) = \det A \cdot \det B$, so $\det(A^2) = (\det A)^2$.

$$
\det(A^2) = (-4)^2 = 16
$$

### 4. Computation of $\det(-A)$

**Property:** Here $c = -1$ for a $3 \times 3$ matrix ($n = 3$):

$$
\det(-A) = (-1)^3 \det A = (-1) \cdot (-4) = 4
$$
