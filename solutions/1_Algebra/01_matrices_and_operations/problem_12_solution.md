# Exercise 12. Formula for a Matrix Power

## Problem Statement

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

---

## Solution

### Part 1. Initial Computations

$$
A^2=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
$$

$$
A^3=A^2 A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}
$$

$$
A^4=A^3 A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}
$$

### Part 2. Conjecture Formulation

From the observed pattern, we conjecture that for all integers $n \ge 1$:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
$$

### Part 3. Proof by Mathematical Induction

- **Base Case ($n=1$):**

$$
A^1 =
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

This matches the formula for $n=1$.

- **Inductive Step:**
  Assume the statement holds for $n$, i.e., $A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}$. We examine $A^{n+1}$:

$$
A^{n+1}=A^n A=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1(1)+n(0) & 1(1)+n(1) \\
0(1)+1(0) & 0(1)+1(1) \\
\end{pmatrix}=
\begin{pmatrix}
1 & n+1 \\
0 & 1 \\
\end{pmatrix}
$$

The induction step is complete. Thus $A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}$ holds for all $n \ge 1$.
