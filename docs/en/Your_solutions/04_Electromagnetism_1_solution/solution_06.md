# Task 06 – Field from a System of Charges

## Problem Statement

Two point charges are given:
- $+q$ at point $(-a, 0)$
- $+2q$ at point $(a, 0)$

1. Determine the field vector $\vec E(x, y)$.
2. Determine the condition for which $\vec E = 0$.
3. Calculate the field for: $a = 0.2$ m, $y = 0.3$ m, $q = 2\ \mu\text{C}$ at $(0, y)$.
4. Investigate the limit $y \gg a$.

## Theory

The electric field from a point charge at a position $\vec{r}$ is:

$$
\vec{E} = k \frac{q}{r^2} \hat{r} = k \frac{q}{r^3} \vec{r}
$$

The total field is the vector sum: $\vec{E}_{total} = \vec{E}_1 + \vec{E}_2$.

## Step-by-Step Solution

### 1. General Field $\vec E(x, y)$
Let $r_1$ be the distance from $(-a, 0)$ and $r_2$ from $(a, 0)$:
- $\vec{r}_1 = (x+a)\hat{i} + y\hat{j}$, $r_1 = \sqrt{(x+a)^2 + y^2}$
- $\vec{r}_2 = (x-a)\hat{i} + y\hat{j}$, $r_2 = \sqrt{(x-a)^2 + y^2}$

$$
\vec{E}(x,y) = kq \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} + \frac{2(x-a)\hat{i} + 2y\hat{j}}{((x-a)^2 + y^2)^{3/2}} \right]
$$

### 2. Zero Field Condition ($\vec E = 0$)
For the field to be zero, the point must be on the x-axis ($y=0$) between the charges. Let the point be $(x, 0)$.

$$
\frac{kq}{(x+a)^2} = \frac{2kq}{(a-x)^2}
$$

Taking the square root:

$$
\frac{1}{x+a} = \frac{\sqrt{2}}{a-x} \implies a - x = \sqrt{2}x + \sqrt{2}a
$$

$$
x = a \frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.17a
$$

### 3. Specific Calculation at $(0, y)$
At $x=0$, $r_1 = r_2 = \sqrt{a^2 + y^2} = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.36$ m.

$$
\vec{E}(0, 0.3) = \frac{kq}{r^3} [ (a\hat{i} + y\hat{j}) + 2(-a\hat{i} + y\hat{j}) ] = \frac{kq}{r^3} (-a\hat{i} + 3y\hat{j})
$$

Substitute $q = 2 \times 10^{-6}$ C:
- $E_x \approx -8.4 \times 10^4$ N/C
- $E_y \approx 3.8 \times 10^5$ N/C

### 4. Limit $y \gg a$
When $y$ is very large, the separation $a$ becomes negligible. The two charges behave like a single charge of $Q = q + 2q = 3q$.

$$
E \approx \frac{k(3q)}{y^2}
$$

## Final Result

The system behaves like a dipole-like configuration at close range but simplifies to a single point charge $3q$ at great distances.

## Interpretation

The "center of the field" is shifted toward the smaller charge because the $+2q$ charge is twice as strong. At far distances, the geometry of the charges is lost, and only the total net charge matters.