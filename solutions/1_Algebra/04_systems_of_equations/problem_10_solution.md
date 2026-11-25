# Exercise 10. A Polynomial Through Three Points

## Problem Statement

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

---

## Solution

### Part 1. Setting Up the Linear System

Substitute points $(x, p(x))$ into polynomial formula:

- Point $(0,1)$: $a(0)^2 + b(0) + c = 1 \implies c = 1$
- Point $(1,3)$: $a(1)^2 + b(1) + c = 3 \implies a + b + c = 3$
- Point $(2,9)$: $a(2)^2 + b(2) + c = 9 \implies 4a + 2b + c = 9$

System for coefficients $(a,b,c)$:

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9.
\end{cases}
$$

### Part 2. Solving the System

Substitute $c=1$ into second and third equations:

$$
\begin{cases}
a+b=2, \\
4a+2b=8 \implies 2a+b=4.
\end{cases}
$$

Subtract first equation from second:

$$
(2a+b) - (a+b) = 4 - 2 \implies a = 2
$$

Substitute $a=2$ into $a+b=2 \implies 2+b=2 \implies b = 0$.

Polynomial formula:

$$
p(x) = 2x^2 + 1
$$

### Part 3. Verification

- $p(0) = 2(0)^2 + 1 = 1$
- $p(1) = 2(1)^2 + 1 = 3$
- $p(2) = 2(2)^2 + 1 = 9$

All points match given coordinates.
