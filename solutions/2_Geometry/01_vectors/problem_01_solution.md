# Exercise 1. Vector Operations and Their Meaning

## Problem Statement

For $u=(2,-1,3)$ and $v=(-1,4,2)$ compute

$$
u+v,\qquad u-v,\qquad 3u-2v.
$$

Then verify that $(u+v)-v=u$, and explain geometrically what adding two vectors means.

---

## Solution

### Part 1. Vector Computations

Given vectors:

$$
u = \begin{pmatrix} 2 \\ -1 \\ 3 \end{pmatrix},\qquad v = \begin{pmatrix} -1 \\ 4 \\ 2 \end{pmatrix}
$$

1. Addition $u+v$:

$$
u+v = \begin{pmatrix} 2+(-1) \\ -1+4 \\ 3+2 \end{pmatrix} = \begin{pmatrix} 1 \\ 3 \\ 5 \end{pmatrix}
$$

2. Subtraction $u-v$:

$$
u-v = \begin{pmatrix} 2-(-1) \\ -1-4 \\ 3-2 \end{pmatrix} = \begin{pmatrix} 3 \\ -5 \\ 1 \end{pmatrix}
$$

3. Linear combination $3u-2v$:

$$
3u-2v = 3\begin{pmatrix} 2 \\ -1 \\ 3 \end{pmatrix} - 2\begin{pmatrix} -1 \\ 4 \\ 2 \end{pmatrix} = \begin{pmatrix} 6 \\ -3 \\ 9 \end{pmatrix} - \begin{pmatrix} -2 \\ 8 \\ 4 \end{pmatrix} = \begin{pmatrix} 8 \\ -11 \\ 5 \end{pmatrix}
$$

### Part 2. Identity Verification

Computing $(u+v)-v$:

$$
(u+v)-v = \begin{pmatrix} 1 \\ 3 \\ 5 \end{pmatrix} - \begin{pmatrix} -1 \\ 4 \\ 2 \end{pmatrix} = \begin{pmatrix} 1-(-1) \\ 3-4 \\ 5-2 \end{pmatrix} = \begin{pmatrix} 2 \\ -1 \\ 3 \end{pmatrix} = u
$$

### Part 3. Geometric Meaning

Geometrically, adding $u+v$ corresponds to applying displacement $u$ followed by displacement $v$ (head-to-tail rule). Subtracting $v$ applies the opposite displacement $-v$, returning to the tip of vector $u$.
