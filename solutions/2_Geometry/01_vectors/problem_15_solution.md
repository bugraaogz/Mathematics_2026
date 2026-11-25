# Exercise 15. Comparing Directions Using the Cosine of the Angle

## Problem Statement

Given

$$
a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3).
$$

For each pair, compute

$$
\frac{u\cdot v}{\|u\|\,\|v\|}.
$$

Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

---

## Solution

### Part 1. Pairwise Cosines

Vector lengths:

$$
\|a\| = \sqrt{1^2+2^2+1^2} = \sqrt{6},\quad \|b\| = \sqrt{2^2+4^2+2^2} = \sqrt{24} = 2\sqrt{6},\quad \|c\| = \sqrt{2^2+0^2+3^2} = \sqrt{13}
$$

1. Pair $(a, b)$:

$$
a \cdot b = 1(2) + 2(4) + 1(2) = 12 \implies \cos\theta_{ab} = \frac{12}{\sqrt{6} \cdot 2\sqrt{6}} = \frac{12}{12} = 1
$$

2. Pair $(a, c)$:

$$
a \cdot c = 1(2) + 2(0) + 1(3) = 5 \implies \cos\theta_{ac} = \frac{5}{\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}} \approx 0.566
$$

3. Pair $(b, c)$:

$$
b \cdot c = 2(2) + 4(0) + 2(3) = 10 \implies \cos\theta_{bc} = \frac{10}{2\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}} \approx 0.566
$$

### Part 2. Ordering by Increasing Angle

- Angle $\theta_{ab} = \arccos(1) = 0^\circ$
- Angles $\theta_{ac} = \theta_{bc} = \arccos\left(\frac{5}{\sqrt{78}}\right) \approx 55.5^\circ$

**Order by increasing angle:** $(a, b) < (a, c) = (b, c)$.

### Part 3. Explanation for Pair $(a, b)$

Notice $b = 2a$. Vector $b$ is a positive scalar multiple of $a$, meaning both vectors point in the exact same direction. Normalizing vector magnitude removes length dependence, yielding $\cos(0^\circ) = 1$.
