## Question

Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check $u=u_{\parallel}+u_{\perp}$ and $u_{\perp}\cdot v=0$. Explain why these are two independent checks of correctness.

## Solution

1. Parallel component:
$$u_{\parallel} = \mathrm{proj}_v u = \frac{u \cdot v}{\|v\|^2} v = \frac{3(1)+4(2)}{1^2+2^2} (1,2) = \frac{11}{5}(1,2) = \left(\frac{11}{5}, \frac{22}{5}\right)$$

2. Perpendicular component:
$$u_{\perp} = u - u_{\parallel} = (3,4) - \left(\frac{11}{5}, \frac{22}{5}\right) = \left(\frac{4}{5}, -\frac{2}{5}\right)$$

3. Checks:
- Sum check: $u_{\parallel} + u_{\perp} = \left(\frac{11}{5} + \frac{4}{5}, \frac{22}{5} - \frac{2}{5}\right) = (3,4) = u$
- Orthogonality check: $u_{\perp} \cdot v = \left(\frac{4}{5}\right)(1) + \left(-\frac{2}{5}\right)(2) = \frac{4-4}{5} = 0$

4. Check 1 verifies vector sum completeness, while Check 2 verifies geometric orthogonality. Together they independently confirm a valid decomposition.
