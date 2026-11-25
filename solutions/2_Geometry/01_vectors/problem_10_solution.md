# Exercise 10. Triangle Area from Vectors

## Problem Statement

The points $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$ form a triangle. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor $\frac12$.

---

## Solution

### Part 1. Vector Construction

$$
\overrightarrow{AB} = \begin{pmatrix} 2 \\ 1 \\ 0 \end{pmatrix},\qquad \overrightarrow{AC} = \begin{pmatrix} 1 \\ 3 \\ 2 \end{pmatrix}
$$

### Part 2. Parallelogram Area

$$
\overrightarrow{AB} \times \overrightarrow{AC} = \det \begin{pmatrix} i & j & k \\ 2 & 1 & 0 \\ 1 & 3 & 2 \end{pmatrix} = i(2 - 0) - j(4 - 0) + k(6 - 1) = \begin{pmatrix} 2 \\ -4 \\ 5 \end{pmatrix}
$$

$$
\mathrm{Area}_{\text{parallelogram}} = \|\overrightarrow{AB} \times \overrightarrow{AC}\| = \sqrt{2^2 + (-4)^2 + 5^2} = \sqrt{4 + 16 + 25} = \sqrt{45} = 3\sqrt{5}
$$

### Part 3. Triangle Area and Factor $\frac{1}{2}$

$$
\mathrm{Area}_{\text{triangle}} = \frac{1}{2} \mathrm{Area}_{\text{parallelogram}} = \frac{3\sqrt{5}}{2}
$$

The factor $\frac{1}{2}$ arises because a triangle formed by two vectors is exactly half of the parallelogram spanned by those same vectors.
