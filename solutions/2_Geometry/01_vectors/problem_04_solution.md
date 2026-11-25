# Exercise 4. Dot Product and Perpendicularity

## Problem Statement

For $u=(1,2,-1)$ and $v=(2,-1,3)$ compute $u\cdot v$ and determine whether the vectors are perpendicular. Then find $a$ so that $w=(2,-1,a)$ is perpendicular to $u$, and check the result.

---

## Solution

### Part 1. Dot Product Computation

$$
u \cdot v = (1)(2) + (2)(-1) + (-1)(3) = 2 - 2 - 3 = -3
$$

Since $u \cdot v = -3 \neq 0$, vectors $u$ and $v$ are **not perpendicular**.

### Part 2. Constructing Perpendicular Vector $w$

For $w = (2, -1, a)^T$ to be perpendicular to $u$, their dot product must equal zero:

$$
u \cdot w = 0 \implies (1)(2) + (2)(-1) + (-1)(a) = 0
$$

$$
2 - 2 - a = 0 \implies a = 0
$$

### Part 3. Verification

For $a = 0$, $w = (2, -1, 0)^T$:

$$
u \cdot w = 1(2) + 2(-1) + (-1)(0) = 2 - 2 + 0 = 0
$$

The zero dot product confirms $w \perp u$.
