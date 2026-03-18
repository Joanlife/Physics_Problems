# Task 07 – Elimination of Time and Acceleration

## Problem Statement
Path equations: $x(t) = 2t^2, y(t) = 3t^3$.
* Eliminate $t$.
* Draw the trajectory (describe).
* Calculate $\vec{v}(t), |\vec{v}(t)|, \vec{a}(t), |\vec{a}(t)|$.
* Is the acceleration constant?

## Theory
To eliminate $t$, solve for $t$ in one equation and substitute into the other. For vectors, use component-wise differentiation.

## Step-by-Step Solution

### 1. Eliminate the Parameter $t$
From $x = 2t^2$, we find $t^2 = \frac{x}{2} \implies t = \left(\frac{x}{2}\right)^{1/2}$.
Substitute into $y = 3t^3$:

$$
y = 3\left(\frac{x}{2}\right)^{3/2}
$$

### 2. Trajectory Description
The trajectory is a semi-cubical parabola. Since $x = 2t^2$, $x$ is always $\geq 0$. As $t$ increases, both $x$ and $y$ increase, creating a curve that starts at the origin and grows steeper as $x$ increases.



### 3. Kinematic Vectors
Velocity is given by differentiating x(t) and y(t):

$$
\vec{v}(t) = \left(\frac{dx}{dt}, \frac{dy}{dt}\right) = (4t, 9t^2)
$$

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}
$$

Acceleration is given by second differenciation of the velocity obtained earlier:

$$
\vec{a}(t) = \left(\frac{dv_x}{dt}, \frac{dv_y}{dt}\right) = (4, 18t)
$$

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}
$$

### 4. Is Acceleration Constant?
No. The $y$-component of acceleration is $18t$, which depends on time. Thus, $\vec{a}(t)$ is not constant.

## Final Result
* **Path:** $y = \frac{3}{2\sqrt{2}}x^{3/2}$
* **Velocity:** $\vec{v} = (4t, 9t^2)$
* **Magnitude:** $t\sqrt{16+81t^2}$
* **Acceleration:** $\vec{a} = (4, 18t)$
* **Constant?** No.