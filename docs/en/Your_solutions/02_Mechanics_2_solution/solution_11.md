# Task 11 – Dynamics with a Time-Dependent Force

## Problem Statement

A particle of mass $m = 3\text{ kg}$ moves in a force field:

$$
\vec{F}(t) = [15t, 3t - 12, -6t^2] \text{ N}
$$

Initial conditions: $\vec{r}_0 = [5, 2, -3]\text{ m}$ and $\vec{v}_0 = [2, 0, 1]\text{ m/s}$. Find $\vec{v}(t)$ and $\vec{r}(t)$.

## Theory

We determine velocity and position by integrating acceleration. From Newton's Second Law:

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

Successive integrations yield:
1. $\vec{v}(t) = \int \vec{a}(t) dt + \vec{C}_1$
2. $\vec{r}(t) = \int \vec{v}(t) dt + \vec{C}_2$

## Step-by-Step Solution

### 1. Acceleration

$$
\vec{a}(t) = \frac{1}{3} [15t, 3t - 12, -6t^2] = [5t, t - 4, -2t^2]
$$

### 2. Velocity

Integrate $\vec{a}(t)$:

$$
\vec{v}(t) = \left[ \frac{5}{2}t^2 + C_{vx}, \frac{1}{2}t^2 - 4t + C_{vy}, -\frac{2}{3}t^3 + C_{vz} \right]
$$

Apply $\vec{v}(0) = [2, 0, 1]$: $C_{vx}=2, C_{vy}=0, C_{vz}=1$.

$$
\vec{v}(t) = \left[ \frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1 \right] \text{ m/s}
$$

### 3. Position

Integrate $\vec{v}(t)$:

$$
\vec{r}(t) = \left[ \frac{5}{6}t^3 + 2t + C_{rx}, \frac{1}{6}t^3 - 2t^2 + C_{ry}, -\frac{1}{6}t^4 + t + C_{rz} \right]
$$

Apply $\vec{r}(0) = [5, 2, -3]$: $C_{rx}=5, C_{ry}=2, C_{rz}=-3$.

$$
\vec{r}(t) = \left[ \frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3 \right] \text{ m/s}
$$

## Final Result

The position vector is:
$$
\vec{r}(t) = \begin{pmatrix} \frac{5}{6}t^3 + 2t + 5 \\ \frac{1}{6}t^3 - 2t^2 + 2 \\ -\frac{1}{6}t^4 + t - 3 \end{pmatrix}
$$

## Interpretation

The motion is non-uniform in all three dimensions. The cubic dependence in $x$ and $y$ and the quartic dependence in $z$ indicate that the particle undergoes increasingly rapid displacement as time progresses due to the time-varying nature of the force.