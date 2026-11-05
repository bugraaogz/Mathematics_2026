# Exercise 13. A Recurrence Written in Matrix Form

## Problem Statement

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

---

## Solution

### Part 1. Computing Powers of $F$

$$
F^2=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
$$

$$
F^3=F^2 F=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

$$
F^4=F^3 F=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}
$$

$$
F^5=F^4 F=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}
$$

### Part 2. Connection with Fibonacci Numbers

Let $f_0=0, f_1=1, f_2=1, f_3=2, f_4=3, f_5=5, f_6=8$ be Fibonacci numbers.
The entries of $F^n$ match consecutive terms of the sequence:

$$
F^n=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix}
$$

### Part 3. Recurrence Step Interpretation

Computing vector multiplication:

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}
$$

Given two consecutive sequence values $b$ and $a$, multiplication by $F$ calculates the next Fibonacci term $a+b$ as the new top element, while shifting the previous top element $a$ to the bottom position for the next iteration.
