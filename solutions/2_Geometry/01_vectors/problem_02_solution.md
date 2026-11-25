# Exercise 2. Distance as the Length of a Vector

## Problem Statement

The points are $A=(1,2,3)$ and $B=(4,-2,6)$.

1. Construct $\overrightarrow{AB}$.
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

---

## Solution

### Part 1. Construction of Vector $\overrightarrow{AB}$

$$
\overrightarrow{AB} = B - A = \begin{pmatrix} 4-1 \\ -2-2 \\ 6-3 \end{pmatrix} = \begin{pmatrix} 3 \\ -4 \\ 3 \end{pmatrix}
$$

### Part 2. Length of $\overrightarrow{AB}$

$$
\|\overrightarrow{AB}\| = \sqrt{3^2 + (-4)^2 + 3^2} = \sqrt{9 + 16 + 9} = \sqrt{34}
$$

### Part 3. Distance Formula

$$
d(A,B) = \sqrt{(x_B - x_A)^2 + (y_B - y_A)^2 + (z_B - z_A)^2} = \sqrt{(4-1)^2 + (-2-2)^2 + (6-3)^2} = \sqrt{34}
$$

### Part 4. Explanation

Both formulas produce the exact same numerical value because displacement vector $\overrightarrow{AB}$ stores the relative coordinate differences between $B$ and $A$. Computing $\|\overrightarrow{AB}\|$ uses the Pythagorean theorem on components $(x_B-x_A, y_B-y_A, z_B-z_A)$, which is identical to the Euclidean distance formula.
