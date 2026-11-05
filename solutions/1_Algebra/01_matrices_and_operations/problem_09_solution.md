# Exercise 9. Composing Transformations

## Problem Statement

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

---

## Solution

### Part 1. Computations

#### Computing $RSx$ (Scale first, then Rotate)

First apply $S$ to $x$:

$$
Sx=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

Now apply $R$ to $Sx$:

$$
RSx=R(Sx)=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

#### Computing $SRx$ (Rotate first, then Scale)

First apply $R$ to $x$:

$$
Rx=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

Now apply $S$ to $Rx$:

$$
SRx=S(Rx)=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

### Part 2. Geometric Interpretation

Comparing the outputs:

$$
RSx=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
\neq
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
=SRx
$$

- In $RSx$, vector $(1,2)$ is first scaled horizontally by factor $2$ to become $(2,2)$, and then rotated by $90^\circ$ counterclockwise into $(-2,2)$.
- In $SRx$, vector $(1,2)$ is first rotated by $90^\circ$ counterclockwise into $(-2,1)$, and then scaled horizontally by factor $2$ into $(-4,1)$.

Because non-uniform scaling expands coordinates along a fixed axis, rotating before versus after scaling alters which geometric axis gets stretched.
