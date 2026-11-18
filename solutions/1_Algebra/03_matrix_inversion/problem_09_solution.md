# Exercise 9. Matrix Equation

## Problem Statement

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

---

## Solution

### Part 1. Deriving the Solution Formula

In $AX = B$, matrix $A$ multiplies $X$ from the left. To isolate $X$, multiply both sides by $A^{-1}$ from the **left**:

$$
A^{-1}(AX) = A^{-1}B \implies (A^{-1}A)X = A^{-1}B \implies IX = A^{-1}B \implies X = A^{-1}B
$$

### Part 2. Computation of $X$

Finding $A^{-1}$:

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
$$

Multiplying $A^{-1}B$:

$$
X=A^{-1}B=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
1(3)+(-2)(2) & 1(1)+(-2)(4) \\
0(3)+1(2) & 0(1)+1(4) \\
\end{pmatrix}=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$

### Part 3. Verification by Computing $AX$

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
1(-1)+2(2) & 1(-7)+2(4) \\
0(-1)+1(2) & 0(-7)+1(4) \\
\end{pmatrix}=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=B
$$

The product equals matrix $B$.
