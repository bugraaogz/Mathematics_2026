# Exercise 14. A Matrix That Is Its Own Inverse

## Problem Statement

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

---

## Solution

### Part 1. Proof that $A^{-1} = A$

We are given $A^2 = I$, which can be written as:

$$
A \cdot A = I
$$

By definition, if $A \cdot B = I$ for a square matrix, then $B$ is the unique inverse $A^{-1}$. Here $B = A$, so:

$$
A^{-1} = A
$$

Alternatively, multiplying $A^2 = I$ on the left by $A^{-1}$:

$$
A^{-1}(A^2) = A^{-1}I \implies (A^{-1}A)A = A^{-1} \implies IA = A^{-1} \implies A = A^{-1}
$$

### Part 2. Constructing an Example

Consider matrix $A$ (a reflection across line $y=x$):

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

Notice $A \neq I$ and $A \neq -I$.

### Part 3. Verification by Multiplication

$$
A^2=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
0(0)+1(1) & 0(1)+1(0) \\
1(0)+0(1) & 1(1)+0(0) \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}=I
$$

This proves $A^2 = I$, verifying $A^{-1} = A$.
