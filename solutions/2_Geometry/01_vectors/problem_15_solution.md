## Question

Given $a=(1,2,1)$, $b=(2,4,2)$, $c=(2,0,3)$. For each pair, compute $\frac{u\cdot v}{\|u\|\,\|v\|}$. Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

## Solution

Vector magnitudes: $\|a\| = \sqrt{6}$, $\|b\| = 2\sqrt{6}$, $\|c\| = \sqrt{13}$.

1. Pairwise cosine values:
$$\frac{a \cdot b}{\|a\|\|b\|} = \frac{12}{\sqrt{6} \cdot 2\sqrt{6}} = \frac{12}{12} = 1 \implies \theta_{ab} = 0^\circ$$

$$\frac{a \cdot c}{\|a\|\|c\|} = \frac{5}{\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}} \approx 0.566 \implies \theta_{ac} \approx 55.5^\circ$$

$$\frac{b \cdot c}{\|b\|\|c\|} = \frac{10}{2\sqrt{6}\sqrt{13}} = \frac{5}{\sqrt{78}} \approx 0.566 \implies \theta_{bc} \approx 55.5^\circ$$

2. Order by increasing angle: $(a,b) < (a,c) = (b,c)$.

3. Explanation for pair $(a,b)$:
Notice $b = 2a$. Since $b$ is a positive scalar multiple of $a$, both vectors point in the exact same direction ($\theta = 0^\circ$). Cosine measures directional alignment, so $\cos(0^\circ) = 1$ regardless of vector magnitudes.
