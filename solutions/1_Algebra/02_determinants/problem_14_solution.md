# Exercise 14. A System of Equations and the Determinant

## Problem Statement

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

---

## Solution

### Part 1. Unique Solution Condition

Computing the determinant of matrix $A$:

$$
\det A = 1(4) - 2(k) = 4 - 2k
$$

The system $Ax=b$ has a unique solution for every vector $b$ if and only if $\det A \neq 0$:

$$
4 - 2k \neq 0 \implies k \neq 2
$$

### Part 2. Exceptional Case $k = 2$

For $k = 2$, matrix $A$ becomes:

$$
A=
\begin{pmatrix}
1 & 2 \\
2 & 4 \\
\end{pmatrix}
$$

The system equations are:

$$
\begin{cases}
x + 2y = b_1, \\
2x + 4y = b_2.
\end{cases}
$$

#### Example with Infinitely Many Solutions

Choose $b = \begin{pmatrix} 1 \\ 2 \end{pmatrix}$:

$$
\begin{cases}
x + 2y = 1, \\
2x + 4y = 2.
\end{cases}
$$

The second equation is $2$ times the first equation, making them consistent and yielding infinitely many solutions.

#### Example with No Solution

Choose $b = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$:

$$
\begin{cases}
x + 2y = 1, \\
2x + 4y = 0 \implies x + 2y = 0.
\end{cases}
$$

This creates the contradiction $1 = 0$, so no solution exists.
