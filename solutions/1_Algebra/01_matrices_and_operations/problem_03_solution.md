# Exercise 3. When Can Matrices Be Multiplied?

## Problem Statement

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

---

## Solution

### Dimension Compatibility Condition

For two matrices $X_{m \times n}$ and $Y_{p \times q}$, the product $XY$ is defined if and only if the number of columns of $X$ equals the number of rows of $Y$ ($n = p$). If defined, the resulting matrix $XY$ has size $m \times q$.

### Analysis of Products

1. **Product $AB$:**
   $A$ is $2 \times 3$ and $B$ is $3 \times 4$. Inner dimensions match ($3 = 3$).
   - **Defined:** Yes. Size: $2 \times 4$.

2. **Product $BA$:**
   $B$ is $3 \times 4$ and $A$ is $2 \times 3$. Inner dimensions do not match ($4 \neq 2$).
   - **Defined:** No.

3. **Product $BC$:**
   $B$ is $3 \times 4$ and $C$ is $4 \times 2$. Inner dimensions match ($4 = 4$).
   - **Defined:** Yes. Size: $3 \times 2$.

4. **Product $CB$:**
   $C$ is $4 \times 2$ and $B$ is $3 \times 4$. Inner dimensions do not match ($2 \neq 3$).
   - **Defined:** No.

5. **Product $AC$:**
   $A$ is $2 \times 3$ and $C$ is $4 \times 2$. Inner dimensions do not match ($3 \neq 4$).
   - **Defined:** No.

6. **Product $CA$:**
   $C$ is $4 \times 2$ and $A$ is $2 \times 3$. Inner dimensions match ($2 = 2$).
   - **Defined:** Yes. Size: $4 \times 3$.

7. **Product $AD$:**
   $A$ is $2 \times 3$ and $D$ is $2 \times 2$. Inner dimensions do not match ($3 \neq 2$).
   - **Defined:** No.

8. **Product $DA$:**
   $D$ is $2 \times 2$ and $A$ is $2 \times 3$. Inner dimensions match ($2 = 2$).
   - **Defined:** Yes. Size: $2 \times 3$.
