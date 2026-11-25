# Exercise 5. Angle Between Vectors

## Problem Statement

Given $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

---

## Solution

### Part 1. Prediction via Dot Product Sign

$$
u \cdot v = (1)(1) + (1)(0) + (0)(1) = 1
$$

Since $u \cdot v = 1 > 0$, the cosine of the angle is positive ($\cos\theta > 0$), predicting an **acute angle** ($0^\circ < \theta < 90^\circ$).

### Part 2. Exact Angle Computation

Vector lengths:

$$
\|u\| = \sqrt{1^2 + 1^2 + 0^2} = \sqrt{2},\qquad \|v\| = \sqrt{1^2 + 0^2 + 1^2} = \sqrt{2}
$$

Cosine formula:

$$
\cos\theta = \frac{u \cdot v}{\|u\|\|v\|} = \frac{1}{\sqrt{2}\sqrt{2}} = \frac{1}{2}
$$

Angle $\theta$:

$$
\theta = \arccos\left(\frac{1}{2}\right) = 60^\circ \quad \left(\frac{\pi}{3} \text{ rad}\right)
$$

### Part 3. Comparison

The exact angle $\theta = 60^\circ$ confirms the initial prediction of an acute angle.
