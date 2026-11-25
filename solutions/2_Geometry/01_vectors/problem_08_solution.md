## Question

Check whether $w=(5,1)$ can be written as $w=au+bv$, where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$ from them, and explain the geometric meaning of the existence of such coefficients.

## Solution

1. System of equations for $a,b$:
$$a(1,1) + b(2,-1) = (5,1) \implies \begin{cases} a + 2b = 5, \\ a - b = 1. \end{cases}$$
Subtracting second equation from first: $3b = 4 \implies b = \frac{4}{3}$.
Substituting back: $a = 1 + \frac{4}{3} = \frac{7}{3}$.

2. Reconstructing $w$:
$$\frac{7}{3}(1,1) + \frac{4}{3}(2,-1) = \left(\frac{7+8}{3}, \frac{7-4}{3}\right) = (5,1) = w$$

3. Geometric meaning:
Since $u$ and $v$ are non-parallel vectors in $\mathbb{R}^2$, they form a basis for 2D space. Any vector $w \in \mathbb{R}^2$ can be uniquely expressed as a linear combination of these basis vectors.
