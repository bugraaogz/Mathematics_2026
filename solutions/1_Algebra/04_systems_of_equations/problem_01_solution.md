# Exercise 1. From a System to a Matrix

## Problem Statement

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

---

## Solution

### Part 1. Matrix Representation $Ax=b$

The system written in matrix form:

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

### Part 2. Identification of Components

- **Coefficient Matrix ($A$):**

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
$$

- **Vector of Unknowns ($x$):**

$$
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
$$

- **Right-Hand Side Vector ($b$):**

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

### Part 3. Row-to-Equation Correspondence

Each row $i$ of matrix $A$ contains the numerical coefficients of variables $x, y, z$ for equation $i$. Evaluating the matrix-vector product $Ax$ computes the dot product of row $i$ with vector $x$, generating the left-hand side of equation $i$, which equals entry $i$ of vector $b$.
