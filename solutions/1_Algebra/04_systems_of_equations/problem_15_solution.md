# Exercise 15. Classifying Three Systems

## Problem Statement

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

---

## Solution

### System 1 Classification

Augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

- **Pivots:** 2 pivots in 2 columns.
- **Classification:** **Exactly one solution** ($(1,1)$).

### System 2 Classification

Augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

- **Pivots:** 1 pivot, 1 free variable ($0=0$).
- **Classification:** **Infinitely many solutions** ($(2-t, t)$).

### System 3 Classification

Augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

- **Contradiction:** Row 2 yields $0 = 1$.
- **Classification:** **No solution** (inconsistent).
