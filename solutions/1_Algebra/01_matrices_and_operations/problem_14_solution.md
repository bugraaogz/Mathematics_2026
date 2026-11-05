# Exercise 14. Rotation Matrices

## Problem Statement

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

---

## Solution

### Part 1. Computing Matrix Product $R(\alpha)R(\beta)$

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}
$$

Performing row-column multiplication:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta - \sin\alpha\sin\beta & -\cos\alpha\sin\beta - \sin\alpha\cos\beta \\
\sin\alpha\cos\beta + \cos\alpha\sin\beta & -\sin\alpha\sin\beta + \cos\alpha\cos\beta \\
\end{pmatrix}
$$

### Part 2. Applying Trigonometric Angle-Sum Identities

Recall the trigonometric sum formulas:

- $\cos(\alpha+\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
- $\sin(\alpha+\beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

Substituting these identities into the product matrix:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}=R(\alpha+\beta)
$$

### Part 3. Geometric Interpretation

Multiplying a vector by $R(\beta)$ rotates it counterclockwise by an angle $\beta$. Multiplying the resulting vector by $R(\alpha)$ rotates it further by an angle $\alpha$. Geometrically, applying two successive rotations by angles $\beta$ and $\alpha$ is identical to performing a single rotation through the total angle $\alpha+\beta$.
