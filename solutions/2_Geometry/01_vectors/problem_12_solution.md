# Exercise 12. A Normal Vector to a Plane

## Problem Statement

Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$. Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

---

## Solution

### Part 1. In-Plane Vectors Construction

$$
u = \overrightarrow{AB} = B - A = \begin{pmatrix} 2-1 \\ 1-0 \\ 0-2 \end{pmatrix} = \begin{pmatrix} 1 \\ 1 \\ -2 \end{pmatrix}
$$

$$
v = \overrightarrow{AC} = C - A = \begin{pmatrix} 0-1 \\ 3-0 \\ 1-2 \end{pmatrix} = \begin{pmatrix} -1 \\ 3 \\ -1 \end{pmatrix}
$$

### Part 2. Normal Vector $n$ via Cross Product

$$
n = u \times v = \det \begin{pmatrix} i & j & k \\ 1 & 1 & -2 \\ -1 & 3 & -1 \end{pmatrix} = i(-1 + 6) - j(-1 - 2) + k(3 + 1) = \begin{pmatrix} 5 \\ 3 \\ 4 \end{pmatrix}
$$

### Part 3. Verification

$$
n \cdot u = 5(1) + 3(1) + 4(-2) = 5 + 3 - 8 = 0
$$

$$
n \cdot v = 5(-1) + 3(3) + 4(-1) = -5 + 9 - 4 = 0
$$

Zero dot products confirm vector $n = (5, 3, 4)^T$ is perpendicular to both in-plane vectors.
