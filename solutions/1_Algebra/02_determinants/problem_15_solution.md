# Exercise 15. Combining Determinant Properties

## Problem Statement

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

---

## Solution

### Part 1. Computation and Properties Used

Using the multiplicative property of determinants:

$$
\det(B^{-1}A^TB) = \det(B^{-1}) \cdot \det(A^T) \cdot \det B
$$

Applying individual determinant properties:

1. **Inverse Property:** $\det(B^{-1}) = \frac{1}{\det B}$ (valid because $\det B = 3 \neq 0$).
2. **Transpose Property:** $\det(A^T) = \det A = -2$.

Substituting these values into the product:

$$
\det(B^{-1}A^TB) = \frac{1}{\det B} \cdot \det A \cdot \det B
$$

### Part 2. Simplification

Because multiplication of real numbers is commutative, $\frac{1}{\det B}$ and $\det B$ cancel:

$$
\det(B^{-1}A^TB) = \left(\frac{1}{3}\right) \cdot (-2) \cdot 3 = -2
$$

### Part 3. Conclusion

The factors involving $B$ cancel out because taking the determinant maps matrix multiplication to real number multiplication, where $\frac{1}{\det B} \cdot \det B = 1$.
