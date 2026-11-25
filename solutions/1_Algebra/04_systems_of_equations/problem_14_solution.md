# Exercise 14. A Small Change in the Right-Hand Side

## Problem Statement

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

---

## Solution

### Part 1. Analysis of System 1

- From equation 3: $3x = 3 \implies x = 1$.
- Substitute $x=1$ into equation 1: $1 + y = 2 \implies y = 1$.
- Check equation 2: $2(1) - 1 = 1$.

System 1 is **consistent** and has unique solution $(x,y) = (1,1)$.

### Part 2. Analysis of System 2

- From equation 3: $3x = 3.1 \implies x = \frac{31}{30} \approx 1.0333$.
- Equations 1 and 2 uniquely determine point $(1,1)$.
- Substituting $(1,1)$ into equation 3 gives $3(1) = 3 \neq 3.1$.

System 2 is **inconsistent** and has **no solution**.

### Part 3. Explanation

Both systems are overdetermined (3 equations in 2 unknowns). In System 1, three line graphs intersect at the exact same point $(1,1)$. Perturbing right-hand side of equation 3 to $3.1$ shifts third line, destroying common intersection point and changing system status from consistent to inconsistent.
