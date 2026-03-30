# Task 10 – Force Field and Power

## Problem Statement

In a force field, a particle of mass $m = 0.5\text{ kg}$ follows the trajectory:

$$
x(t) = 5t^2 - t, \quad y(t) = 2t^3, \quad z(t) = -3t + 2
$$

Find the time dependence of:
1. Velocity $\vec{v}(t)$
2. Momentum $\vec{p}(t)$
3. Acceleration $\vec{a}(t)$
4. Force $\vec{F}(t)$
5. Power $P(t)$

## Theory

Kinematics and dynamics in three dimensions are handled by differentiating the position vector $\vec{r}(t) = [x(t), y(t), z(t)]$:

* **Velocity**: $\vec{v} = \frac{d\vec{r}}{dt}$
* **Acceleration**: $\vec{a} = \frac{d\vec{v}}{dt}$
* **Momentum**: $\vec{p} = m\vec{v}$
* **Force**: $\vec{F} = m\vec{a}$ (Newton's Second Law)
* **Power**: $P = \vec{F} \cdot \vec{v}$ (Dot product of force and velocity)

## Step-by-Step Solution

### 1. Velocity
Differentiate each component with respect to $t$:

$$
v_x = \frac{dx}{dt} = 10t - 1, \quad v_y = \frac{dy}{dt} = 6t^2, \quad v_z = \frac{dz}{dt} = -3
$$

$$
\vec{v}(t) = [10t - 1, 6t^2, -3] \text{ m/s}
$$

### 2. Momentum
Multiply velocity by $m = 0.5\text{ kg}$:

$$
\vec{p}(t) = 0.5 \cdot [10t - 1, 6t^2, -3] = [5t - 0.5, 3t^2, -1.5] \text{ kg}\cdot\text{m/s}
$$

### 3. Acceleration
Differentiate velocity with respect to $t$:

$$
a_x = \frac{dv_x}{dt} = 10, \quad a_y = \frac{dv_y}{dt} = 12t, \quad a_z = \frac{dv_z}{dt} = 0
$$

$$
\vec{a}(t) = [10, 12t, 0] \text{ m/s}^2
$$

### 4. Force
Multiply acceleration by $m = 0.5\text{ kg}$:

$$
\vec{F}(t) = 0.5 \cdot [10, 12t, 0] = [5, 6t, 0] \text{ N}
$$

### 5. Power
Calculate the dot product $P = F_x v_x + F_y v_y + F_z v_z$:

$$
P(t) = 5(10t - 1) + 6t(6t^2) + 0(-3)
$$

$$
P(t) = 50t - 5 + 36t^3 \text{ W}
$$

## Final Result

* $\vec{v}(t) = [10t - 1, 6t^2, -3]$
* $\vec{a}(t) = [10, 12t, 0]$
* $\vec{F}(t) = [5, 6t, 0]$
* $P(t) = 36t^3 + 50t - 5$

## Interpretation

The force in the x-direction is constant, while the force in the y-direction grows linearly over time. Consequently, the power—the rate at which the field does work on the particle—grows cubically as the particle speeds up.