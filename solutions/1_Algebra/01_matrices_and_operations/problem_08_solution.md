# Exercise 8. Row Operations and Their Reversibility

## Problem Statement

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

---

## Solution

### Initial Matrix

$$
A_0=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

### Step 1. $R_2\leftarrow R_2-2R_1$

Subtracting twice row 1 from row 2:

$$
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

- **Reversing Operation:** $R_2 \leftarrow R_2 + 2R_1$

### Step 2. $R_3\leftarrow R_3+R_1$

Adding row 1 to row 3:

$$
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

- **Reversing Operation:** $R_3 \leftarrow R_3 - R_1$

### Step 3. Interchange $R_2$ and $R_3$

Swapping row 2 and row 3:

$$
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

- **Reversing Operation:** Interchange $R_2$ and $R_3$ (applying the swap again).
