# Exercise 11. Decomposition into Parallel and Perpendicular Components

## Problem Statement

Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check

$$
u=u_{\parallel}+u_{\perp},\qquad u_{\perp}\cdot v=0.
$$

Explain why these are two independent checks of correctness.

---

## Solution

### Part 1. Component Construction

Parallel component $u_{\parallel}$:

$$
u \cdot v = 3(1) + 4(2) = 11,\qquad \|v\|^2 = 1^2 + 2^2 = 5
$$

$$
u_{\parallel} = \mathrm{proj}_v u = \frac{11}{5}\begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix} \frac{11}{5} \\ \frac{22}{5} \end{pmatrix}
$$

Perpendicular component $u_{\perp}$:

$$
u_{\perp} = u - u_{\parallel} = \begin{pmatrix} 3 \\ 4 \end{pmatrix} - \begin{pmatrix} \frac{11}{5} \\ \frac{22}{5} \end{pmatrix} = \begin{pmatrix} \frac{4}{5} \\ -\frac{2}{5} \end{pmatrix}
$$

### Part 2. Verification

1. Vector Sum:

$$
u_{\parallel} + u_{\perp} = \begin{pmatrix} \frac{11}{5} \\ \frac{22}{5} \end{pmatrix} + \begin{pmatrix} \frac{4}{5} \\ -\frac{2}{5} \end{pmatrix} = \begin{pmatrix} \frac{15}{5} \\ \frac{20}{5} \end{pmatrix} = \begin{pmatrix} 3 \\ 4 \end{pmatrix} = u
$$

2. Orthogonality:

$$
u_{\perp} \cdot v = \left(\frac{4}{5}\right)(1) + \left(-\frac{2}{5}\right)(2) = \frac{4 - 4}{5} = 0
$$

### Part 3. Explanation

- Check 1 ($u = u_{\parallel} + u_{\perp}$) confirms algebraic completeness (no component is lost).
- Check 2 ($u_{\perp} \cdot v = 0$) confirms directional orthogonality.
Together, they independently verify a valid orthogonal decomposition.
