# Exercise 11. When Do Matrices Commute?

## Problem Statement

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

---

## Solution

### Part 1. Computing $AB$ and $BA$

Computing $AB$:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix}
$$

Computing $BA$:

$$
BA=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}
$$

### Part 2. Equating $AB = BA$

Equating corresponding entries:

1. Top-left entry: $a + c = a \implies c = 0$
2. Top-right entry: $b + d = a + b \implies d = a$
3. Bottom-left entry: $c = c$ (always true)
4. Bottom-right entry: $d = c + d \implies c = 0$

### Part 3. General Form of Matrix $B$

The condition $AB=BA$ holds if and only if $c=0$ and $d=a$, with $b$ taking any real value. The general form of all commuting matrices $B$ is:

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}
$$

where $a, b \in \mathbb{R}$.
