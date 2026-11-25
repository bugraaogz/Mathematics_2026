# Exercise 13. Do Four Points Lie in One Plane?

## Problem Statement

Given

$$
A=(0,0,0),\qquad B=(1,2,0),\qquad C=(0,1,1),\qquad D=(2,5,1).
$$

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Find $n=\overrightarrow{AB}\times\overrightarrow{AC}$.
3. Construct $\overrightarrow{AD}$ and check whether $\overrightarrow{AD}\cdot n=0$.
4. Based on this, decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

---

## Solution

### Part 1 & 2. In-Plane Vectors and Normal Vector $n$

$$
\overrightarrow{AB} = \begin{pmatrix} 1 \\ 2 \\ 0 \end{pmatrix},\qquad \overrightarrow{AC} = \begin{pmatrix} 0 \\ 1 \\ 1 \end{pmatrix}
$$

$$
n = \overrightarrow{AB} \times \overrightarrow{AC} = \det \begin{pmatrix} i & j & k \\ 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} = i(2 - 0) - j(1 - 0) + k(1 - 0) = \begin{pmatrix} 2 \\ -1 \\ 1 \end{pmatrix}
$$

### Part 3. Vector $\overrightarrow{AD}$ and Dot Product

$$
\overrightarrow{AD} = D - A = \begin{pmatrix} 2 \\ 5 \\ 1 \end{pmatrix}
$$

$$
\overrightarrow{AD} \cdot n = 2(2) + 5(-1) + 1(1) = 4 - 5 + 1 = 0
$$

### Part 4. Coplanarity Decision

Since $\overrightarrow{AD} \cdot n = 0$, vector $\overrightarrow{AD}$ is perpendicular to normal vector $n$, meaning point $D$ lies entirely within the plane spanned by points $A, B, C$.
