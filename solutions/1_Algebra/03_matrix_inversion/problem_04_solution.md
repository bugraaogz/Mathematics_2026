# Exercise 4. Gauss–Jordan

## Problem Statement

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

---

## Solution

### Part 1. Gauss–Jordan Elimination

Set up the augmented matrix $[A \mid I]$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

#### Step 1. $R_2 \leftarrow R_2 - 3R_1$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

#### Step 2. $R_2 \leftarrow -1 \cdot R_2$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

#### Step 3. $R_1 \leftarrow R_1 - 2R_2$

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

The left side has reached $I$, so the inverse is:

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
$$

### Part 2. Explanation

Row operations correspond to multiplying by elementary matrices $E_k \cdots E_2 E_1$. When these operations transform $A$ into $I$:

$$
(E_k \cdots E_1) A = I \implies E_k \cdots E_1 = A^{-1}
$$

Applying the exact same operations simultaneously to $I$ yields $(E_k \cdots E_1) I = A^{-1}$ on the right side.
