# Task 03 – Path Intersection

## Problem Statement
Two objects move along paths:
$A(t) = (2+t, 8-3t)$
$B(t) = (2t-1, 2t+2)$
Determine if their paths intersect. If yes, Determine when and where they will collide. If not, find the minimum distance and when it occurs.

## Theory
An **intersection** occurs if the sets of coordinates $(x, y)$ occupied by the paths share a point, even at different times $t_1$ and $t_2$. A **collision** occurs only if they occupy the same point at the same time $t$.

## Step-by-Step Solution

### 1. Checking for Collision
For a collision, $A(t) = B(t)$:

$$
2 + t = 2t - 1 \implies t = 3
$$

$$
8 - 3t = 2t + 2 \implies 5t = 6 \implies t = 1.2
$$

Since $3 \neq 1.2$, the objects do not collide.

### 2. Checking for Path Intersection
We set $A(t_1) = B(t_2)$:
1) $2 + t_1 = 2t_2 - 1$
2) $8 - 3t_1 = 2t_2 + 2$

From (1): $t_1 = 2t_2 - 3$. Substitute into (2):

$$
8 - 3(2t_2 - 3) = 2t_2 + 2
$$

$$
8 - 6t_2 + 9 = 2t_2 + 2 \implies 8t_2 = 15 \implies t_2 = 1.875
$$

$$
t_1 = 2(1.875) - 3 = 0.75
$$

The paths intersect at $t_1 = 0.75$ and $t_2 = 1.875$. The coordinates are $(2.75, 5.75)$.

### 3. Minimum Distance
The distance $D(t)$ squared is:

$$
D^2(t) = (x_A - x_B)^2 + (y_A - y_B)^2
$$

$$
x_A - x_B = (2+t) - (2t-1) = 3-t
$$

$$
y_A - y_B = (8-3t) - (2t+2) = 6-5t
$$

$$
f(t) = D^2(t) = (3-t)^2 + (6-5t)^2 = 9 - 6t + t^2 + 36 - 60t + 25t^2
$$

$$
f(t) = 26t^2 - 66t + 45
$$

To minimize, $f'(t) = 52t - 66 = 0 \implies t = \frac{66}{52} \approx 1.27 \text{ s}$.

$$
D_{min} = \sqrt{26(1.27)^2 - 66(1.27) + 45} \approx 1.76 \text{ units}
$$

## Final Result
* **Collision:** No.
* **Intersection:** Yes, at $(2.75, 5.75)$.
* **Min Distance:** $1.76$ at $t \approx 1.27 \text{ s}$.

## Interpretation
The paths cross in space, but the objects pass through that point at different times.