# Exercise 3. Vector Normalization

## Problem Statement

For $v=(3,4)$ find a unit vector $e$ with the same direction and orientation. Check that $\|e\|=1$, reconstruct $v$ in the form $v=\|v\|e$, and explain what changes during normalization and what remains unchanged.

---

## Solution

### Part 1. Normalization

Magnitude of $v = (3,4)^T$:

$$
\|v\| = \sqrt{3^2 + 4^2} = \sqrt{25} = 5
$$

Unit vector $e$:

$$
e = \frac{v}{\|v\|} = \frac{1}{5}\begin{pmatrix} 3 \\ 4 \end{pmatrix} = \begin{pmatrix} \frac{3}{5} \\ \frac{4}{5} \end{pmatrix}
$$

### Part 2. Length Check and Reconstruction

Checking length of $e$:

$$
\|e\| = \sqrt{\left(\frac{3}{5}\right)^2 + \left(\frac{4}{5}\right)^2} = \sqrt{\frac{9}{25} + \frac{16}{25}} = \sqrt{1} = 1
$$

Reconstructing $v$:

$$
\|v\|e = 5 \begin{pmatrix} \frac{3}{5} \\ \frac{4}{5} \end{pmatrix} = \begin{pmatrix} 3 \\ 4 \end{pmatrix} = v
$$

### Part 3. Explanation

- **What changes:** The length (magnitude) of vector $v$ changes from $5$ to $1$.
- **What remains unchanged:** The spatial direction and orientation remain identical.
