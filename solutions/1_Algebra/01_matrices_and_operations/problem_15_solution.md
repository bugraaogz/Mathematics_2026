# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Problem Statement

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

---

## Solution

### Path 1. Computing $(AB)C$

First compute product $AB$:

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
1(1)+2(2)+0(-1) & 1(0)+2(1)+0(3) \\
0(1)+1(2)+1(-1) & 0(0)+1(1)+1(3) \\
\end{pmatrix}=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

Now compute $(AB)C$:

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}=
\begin{pmatrix}
5(2)+2(0) & 5(1)+2(-1) \\
1(2)+4(0) & 1(1)+4(-1) \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

### Path 2. Computing $A(BC)$

First compute product $BC$:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}=
\begin{pmatrix}
1(2)+0(0) & 1(1)+0(-1) \\
2(2)+1(0) & 2(1)+1(-1) \\
-1(2)+3(0) & -1(1)+3(-1) \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}
$$

Now compute $A(BC)$:

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}=
\begin{pmatrix}
1(2)+2(4)+0(-2) & 1(1)+2(1)+0(-4) \\
0(2)+1(4)+1(-2) & 0(1)+1(1)+1(-4) \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

### Comparison of Operation Counts and Associativity Meaning

- Both evaluation paths yield the identical resulting matrix:

$$
(AB)C = A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}
$$

- **Scalar Multiplications Count:**
  - **Path 1 ($(AB)C$):** $AB$ requires $2 \times 3 \times 2 = 12$ multiplications; then $(AB)C$ requires $2 \times 2 \times 2 = 8$ multiplications. Total = $20$ scalar multiplications.
  - **Path 2 ($A(BC)$):** $BC$ requires $3 \times 2 \times 2 = 12$ multiplications; then $A(BC)$ requires $2 \times 3 \times 2 = 12$ multiplications. Total = $24$ scalar multiplications.

Associativity guarantees that grouping of factors does not alter the mathematical outcome. However, choosing the order of pairwise multiplications can alter computational cost depending on matrix sizes.
