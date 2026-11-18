# Exercise 13. Undoing a Composite Transformation

## Problem Statement

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

---

## Solution

### Method 1. Computing $T$, then $T^{-1}$

First compute $T = HS$:

$$
T=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

$\det T = 2(1) - 1(0) = 2$. Computing $T^{-1}$:

$$
T^{-1}=\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}
$$

### Method 2. Using $(HS)^{-1} = S^{-1}H^{-1}$

Individual inverses:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$

Multiplying $S^{-1}H^{-1}$:

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}
$$

### Part 3. Computing Incorrect Order $H^{-1}S^{-1}$

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1 \\
\end{pmatrix} \neq T^{-1}
$$

### Part 4. Rule Explanation

In composition $HS$, matrix $S$ is applied first, followed by $H$. To undo the sequence, one must reverse the last operation first ($H^{-1}$), and then undo the initial operation ($S^{-1}$). Thus $(HS)^{-1} = S^{-1}H^{-1}$.
