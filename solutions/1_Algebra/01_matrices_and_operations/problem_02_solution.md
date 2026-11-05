# Exercise 2. Addition and Scalar Multiplication

## Problem Statement

For

$$A= \begin{pmatrix} 1 & 2 \\ -1 & 3 \\ \end{pmatrix},\qquad B= \begin{pmatrix} 4 & -2 \\ 0 & 5 \\ \end{pmatrix}$$

compute

$$A+B,\qquad A-B,\qquad 3A-2B.$$

Explain why matrix addition is possible only for matrices of the same size.

---

## Solution

### Part 1. Computations

#### Computation of $A+B$

Matrix addition is performed entry by entry:

$$A+B= \begin{pmatrix} 1+4 & 2+(-2) \\ -1+0 & 3+5 \\ \end{pmatrix}= \begin{pmatrix} 5 & 0 \\ -1 & 8 \\ \end{pmatrix}$$

#### Computation of $A-B$

Matrix subtraction is performed entry by entry:

$$A-B= \begin{pmatrix} 1-4 & 2-(-2) \\ -1-0 & 3-5 \\ \end{pmatrix}= \begin{pmatrix} -3 & 4 \\ -1 & -2 \\ \end{pmatrix}$$

#### Computation of $3A-2B$

First compute the scalar multiples $3A$ and $2B$:

$$3A= \begin{pmatrix} 3(1) & 3(2) \\ 3(-1) & 3(3) \\ \end{pmatrix}= \begin{pmatrix} 3 & 6 \\ -3 & 9 \\ \end{pmatrix}$$

$$2B= \begin{pmatrix} 2(4) & 2(-2) \\ 2(0) & 2(5) \\ \end{pmatrix}= \begin{pmatrix} 8 & -4 \\ 0 & 10 \\ \end{pmatrix}$$

Subtracting $2B$ from $3A$:

$$3A-2B= \begin{pmatrix} 3-8 & 6-(-4) \\ -3-0 & 9-10 \\ \end{pmatrix}= \begin{pmatrix} -5 & 10 \\ -3 & -1 \\ \end{pmatrix}$$

### Part 2. Explanation of Size Requirement for Matrix Addition

Matrix addition is defined element-wise: $(A+B)_{ij} = a_{ij} + b_{ij}$. If two matrices have different dimensions, there exist entries in one matrix that have no corresponding position in the other matrix. Therefore, matrix addition is defined if and only if both matrices have the exact same dimensions.
