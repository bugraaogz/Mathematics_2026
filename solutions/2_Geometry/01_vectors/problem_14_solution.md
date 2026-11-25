# Exercise 14. Closest Point on a Line

## Problem Statement

Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$. Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

---

## Solution

### Part 1. Finding Closest Point $Q$

Let vector $u = \overrightarrow{OP} = (4,1)^T$. The closest point $Q$ on the line is given by orthogonal projection of $u$ onto direction $v$:

$$
u \cdot v = 4(1) + 1(2) = 6,\qquad \|v\|^2 = 1^2 + 2^2 = 5
$$

$$
Q = \mathrm{proj}_v u = \frac{6}{5}\begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix} \frac{6}{5} \\ \frac{12}{5} \end{pmatrix}
$$

### Part 2. Distance from $P$ to Line

Vector $\overrightarrow{QP}$:

$$
\overrightarrow{QP} = P - Q = \begin{pmatrix} 4 \\ 1 \end{pmatrix} - \begin{pmatrix} \frac{6}{5} \\ \frac{12}{5} \end{pmatrix} = \begin{pmatrix} \frac{14}{5} \\ -\frac{7}{5} \end{pmatrix}
$$

Distance:

$$
d = \|\overrightarrow{QP}\| = \sqrt{\left(\frac{14}{5}\right)^2 + \left(-\frac{7}{5}\right)^2} = \sqrt{\frac{196 + 49}{25}} = \sqrt{\frac{245}{25}} = \frac{7\sqrt{5}}{5}
$$

### Part 3. Perpendicularity Verification

$$
\overrightarrow{QP} \cdot v = \left(\frac{14}{5}\right)(1) + \left(-\frac{7}{5}\right)(2) = \frac{14 - 14}{5} = 0
$$

Zero dot product confirms vector $\overrightarrow{QP}$ is orthogonal to direction $v$, proving $Q$ is the unique closest point.
