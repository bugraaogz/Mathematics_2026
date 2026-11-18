# Exercise 1. Definition of the Inverse

## Problem Statement

For

$$A= \begin{pmatrix} 2 & 1 \\ 1 & 1 \\ \end{pmatrix},\qquad B= \begin{pmatrix} 1 & -1 \\ -1 & 2 \\ \end{pmatrix}$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

---

## Solution

### Part 1. Computation of $AB$

$$AB= \begin{pmatrix} 2 & 1 \\ 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & -1 \\ -1 & 2 \\ \end{pmatrix}= \begin{pmatrix} 2(1)+1(-1) & 2(-1)+1(2) \\ 1(1)+1(-1) & 1(-1)+1(2) \\ \end{pmatrix}= \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix}$$

### Part 2. Computation of $BA$

$$BA= \begin{pmatrix} 1 & -1 \\ -1 & 2 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 1 & 1 \\ \end{pmatrix}= \begin{pmatrix} 1(2)+(-1)(1) & 1(1)+(-1)(1) \\ -1(2)+2(1) & -1(1)+2(1) \\ \end{pmatrix}= \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix}$$

### Part 3. Relation to Definition of Inverse

By definition, a matrix $B$ is the inverse of $A$ ($B = A^{-1}$) if and only if $AB = BA = I$, where $I$ is the identity matrix. Since both products equal the $2 \times 2$ identity matrix:

$$AB = BA = \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix}$$

we conclude directly from the definition that $B = A^{-1}$.
