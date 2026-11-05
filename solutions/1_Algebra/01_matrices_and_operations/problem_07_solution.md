# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Problem Statement

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

---

## Solution

### Part 1. Computations

Here $I$ is the $2 \times 2$ identity matrix and $0$ is the $2 \times 2$ zero matrix:

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad 0=
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
$$

#### Computations with $I$ and $0$

$$
AI=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
IA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
A+0=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}+
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

#### Matrix Powers $A^2$ and $A^3$

$$
A^2=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

$$
A^3=A^2 A=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

### Part 2. Roles of $I$ and $0$ and Power Pattern

- **Role of $I$:** Acts as the multiplicative identity element ($AI = IA = A$).
- **Role of $0$:** Acts as the additive identity element ($A + 0 = A$).
- **Pattern in Powers of $A$:**
  For $A^1 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}$, $A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}$, $A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}$.
  The diagonal entries follow $2^n$, while the top-right entry follows $n \cdot 2^{n-1}$. Thus:

$$
A^n=
\begin{pmatrix}
2^n & n \cdot 2^{n-1} \\
0 & 2^n \\
\end{pmatrix}
$$
