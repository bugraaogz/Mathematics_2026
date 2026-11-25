## Question

Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$. Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

## Solution

1. Let $u = \overrightarrow{OP} = (4,1)$. Closest point $Q$ on the line:
$$Q = \mathrm{proj}_v u = \frac{4(1)+1(2)}{1^2+2^2} (1,2) = \frac{6}{5}(1,2) = \left(\frac{6}{5}, \frac{12}{5}\right)$$

2. Displacement vector $\overrightarrow{QP} = P - Q = \left(4 - \frac{6}{5}, 1 - \frac{12}{5}\right) = \left(\frac{14}{5}, -\frac{7}{5}\right)$.

Distance:
$$d = \|\overrightarrow{QP}\| = \sqrt{\left(\frac{14}{5}\right)^2 + \left(-\frac{7}{5}\right)^2} = \sqrt{\frac{196+49}{25}} = \frac{\sqrt{245}}{5} = \frac{7\sqrt{5}}{5}$$

3. Perpendicularity verification:
$$\overrightarrow{QP} \cdot v = \left(\frac{14}{5}\right)(1) + \left(-\frac{7}{5}\right)(2) = \frac{14 - 14}{5} = 0$$
