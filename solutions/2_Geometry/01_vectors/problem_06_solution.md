# Exercise 6. Projection and Perpendicular Component

## Problem Statement

Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute

$$
r=u-\mathrm{proj}_v\,u
$$

and verify that $r\cdot v=0$. Explain this result geometrically.

---

## Solution

### Part 1. Projection Computation

$$
u \cdot v = 4(1) + 2(1) = 6,\qquad \|v\|^2 = 1^2 + 1^2 = 2
$$

$$
\mathrm{proj}_v u = \frac{u \cdot v}{\|v\|^2} v = \frac{6}{2} \begin{pmatrix} 1 \\ 1 \end{pmatrix} = \begin{pmatrix} 3 \\ 3 \end{pmatrix}
$$

### Part 2. Perpendicular Component $r$

$$
r = u - \mathrm{proj}_v u = \begin{pmatrix} 4 \\ 2 \end{pmatrix} - \begin{pmatrix} 3 \\ 3 \end{pmatrix} = \begin{pmatrix} 1 \\ -1 \end{pmatrix}
$$

### Part 3. Perpendicularity Verification

$$
r \cdot v = (1)(1) + (-1)(1) = 1 - 1 = 0
$$

### Part 4. Geometric Meaning

Vector $u$ is decomposed into two orthogonal components: $\mathrm{proj}_v u$ (parallel to $v$) and $r$ (orthogonal to $v$).
