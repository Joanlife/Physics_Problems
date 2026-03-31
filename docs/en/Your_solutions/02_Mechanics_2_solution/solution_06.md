# Task 06 – Energy Dissipation: Bouncing Ball

## Problem Statement

A tennis ball is dropped from a height of $2.0\text{ m}$. After each bounce, it loses $30\%$ of its mechanical energy. To what height does it rise after the second bounce?

## Theory

The mechanical energy of the ball at its peak height $h$ is purely potential:
$$
E = mgh
$$

If the ball loses $30\%$ of its energy, it retains $70\%$ ($0.70$) of its energy. Since m(mass) and g(gravity) don't change, Energy(E) is directly proportional to the height(h)  $E \propto h$, the height reached after a bounce is directly proportional to the energy remaining:
$$
h_{new} = 0.70 \cdot h_{old}
$$

## Step-by-Step Solution

### 1. Energy After First Bounce

Initial height $h_0 = 2.0\text{ m}$.
Energy after 1st bounce $E_1 = 0.70 E_0$.
Height after 1st bounce:

$$
h_1 = 0.70 \cdot h_0 = 0.70 \cdot 2.0 = 1.4\text{ m}
$$

### 2. Energy After Second Bounce

The ball now drops from $h_1$ and loses another $30\%$ of its remaining energy upon the second impact.
Energy after 2nd bounce $E_2 = 0.70 E_1 $.
Height after 2nd bounce:

$$
h_2 = 0.70 \cdot h_1 = 0.70 \cdot 1.4 = 0.98\text{ m}
$$

## Final Result

The ball rises to a height of $0.98\text{ m}$ after the second bounce.

## Interpretation

The height follows a geometric progression $h_n = h_0 \cdot (r)^n$, where $r$ is the energy retention coefficient (0.70) and $n$ is the number of bounces. Even though the percentage lost is constant, the absolute height lost decreases with each bounce as the total energy of the system diminishes.