# Task 12 – Work and Energy with a Constant Force

## Problem Statement

A constant force $\vec{F} = [6, 2]\text{ N}$ acts on a body of mass $m = 2\text{ kg}$. 
The body starts with an initial velocity $\vec{v}(0) = [1, -1]\text{ m/s}$ from the point $\vec{r}(0) = [0, 0]\text{ m}$.

1. Determine $\vec{a}(t)$
2. Determine $\vec{v}(t)$ using integration
3. Determine $\vec{r}(t)$ using integration
4. Calculate the work done by the force at time $t = 3\text{ s}$
5. Check the consistency with the work-energy theorem

## Theory

Newton's Second Law states that $\vec{F} = m\vec{a}$. Since the force and mass are constant, the acceleration is also constant. 

We find velocity and position by performing indefinite integration of the acceleration and velocity vectors respectively. The constants of integration are determined by the initial conditions:

$$
\vec{v}(t) = \int \vec{a}(t) dt
$$

$$
\vec{r}(t) = \int \vec{v}(t) dt
$$

## Step-by-Step Solution

### 1. Acceleration
Using $\vec{a} = \frac{\vec{F}}{m}$:

$$
\vec{a} = \frac{[6, 2]}{2} = [3, 1] \text{ m/s}^2
$$

### 2. Velocity via Integration
We integrate the acceleration vector with respect to time:

$$
\vec{v}(t) = \int [3, 1] dt = [3t + C_x, t + C_y]
$$

Using the initial condition $\vec{v}(0) = [1, -1]$:
* $3(0) + C_x = 1 \implies C_x = 1$
* $0 + C_y = -1 \implies C_y = -1$

$$
\vec{v}(t) = [3t + 1, t - 1] \text{ m/s}
$$

### 3. Position via Integration
We integrate the velocity vector with respect to time:

$$
\vec{r}(t) = \int [3t + 1, t - 1] dt = \left[ \frac{3}{2}t^2 + t + D_x, \frac{1}{2}t^2 - t + D_y \right]
$$

Using the initial condition $\vec{r}(0) = [0, 0]$:
* $0 + 0 + D_x = 0 \implies D_x = 0$
* $0 - 0 + D_y = 0 \implies D_y = 0$

$$
\vec{r}(t) = [1.5t^2 + t, 0.5t^2 - t] \text{ m}
$$

### 4. Work Done at $t = 3\text{ s}$
First, find the displacement vector $\Delta\vec{r}$ at $t = 3$:

$$
x(3) = 1.5(3)^2 + 3 = 13.5 + 3 = 16.5\text{ m}
$$

$$
y(3) = 0.5(3)^2 - 3 = 4.5 - 3 = 1.5\text{ m}
$$

$$
W = \vec{F} \cdot \Delta\vec{r} = [6, 2] \cdot [16.5, 1.5]
$$

$$
W = 6(16.5) + 2(1.5) = 99 + 3 = 102\text{ J}
$$

### 5. Work-Energy Theorem Verification
Initial kinetic energy ($t=0$):
$v(0)^2 = 1^2 + (-1)^2 = 2$

$$
K_i = \frac{1}{2} m v_0^2 = \frac{1}{2} (2)(2) = 2\text{ J}
$$

Final kinetic energy ($t=3$):
$\vec{v}(3) = [3(3)+1, 3-1] = [10, 2]$
$v(3)^2 = 10^2 + 2^2 = 104$

$$
K_f = \frac{1}{2} m v_f^2 = \frac{1}{2} (2)(104) = 104\text{ J}
$$

Change in kinetic energy:
$\Delta K = 104 - 2 = 102\text{ J}$

Since $W = \Delta K$, the theorem is verified,whereby it states that the total work done on an object equals its change in kinetic energy.

## Final Result

* $\vec{a} = [3, 1]\text{ m/s}^2$
* $\vec{v}(t) = [3t + 1, t - 1]\text{ m/s}$
* $\vec{r}(t) = [1.5t^2 + t, 0.5t^2 - t]\text{ m}$
* $W = 102\text{ J}$

## Interpretation


The constant force results in a parabolic trajectory. The integration constants $C$ and $D$ physically represent the "starting state" of the system. Even with a positive force in the $y$-direction, the particle initially moves in the negative $y$-direction because of its initial velocity, before the force eventually reverses its direction.