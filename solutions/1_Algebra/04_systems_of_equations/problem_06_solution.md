# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Problem Statement

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

---

## Solution

### Part 1. Gaussian Elimination

Set up augmented matrix $[A \mid b]$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

Apply $R_2 \leftarrow R_2 - a R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

### Part 2. Parameter Cases Analysis

1. **Case $4 - 2a \neq 0 \implies a \neq 2$:**
   Row 2 becomes $0x + 0y = 4 - 2a \neq 0$, producing a contradiction. The system has **no solution**.

2. **Case $4 - 2a = 0 \implies a = 2$:**
   Row 2 becomes $0 = 0$. The system reduces to single equation $x+y=2$, yielding **infinitely many solutions** ($(2-t, t)$ for $t \in \mathbb{R}$).

### Part 3. Excluded Case Explanation

The case of **exactly one solution** can **never occur** for any value of $a$. The determinant of coefficient matrix $A$ is:

$$
\det A = \det
\begin{pmatrix}
1 & 1 \\
a & a \\
\end{pmatrix} = 1(a) - 1(a) = 0
$$

Since $\det A = 0$ for all real numbers $a$, the coefficient matrix is singular for all $a$, preventing the existence of a unique solution.
