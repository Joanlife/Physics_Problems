# Task 01 – Projectile Motion

## Problem Statement
A projectile is fired from the ground with an initial velocity $v_0 = 100 \text{ m/s}$ at an angle $\theta = 37^\circ$ above the horizontal. Assuming no air resistance:
* Derive the differential equations of motion in the horizontal and vertical directions.
* Determine the time of flight $t_f$.
* Determine the maximum height $H$.
* Determine the range $R$.

## Theory
Projectile motion is a case of two-dimensional kinematics where the only acceleration acting on the object is gravity $\vec{g}$, acting vertically downward. We decompose the initial velocity into components:

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

Neglecting air resistance, the horizontal acceleration is zero, and the vertical acceleration is constant.

## Step-by-Step Solution

# Task 01 – Projectile Motion (Detailed Derivations)

## Problem Statement
A projectile is fired from $y=0$ with $v_0 = 100 \text{ m/s}$ at $\theta = 37^\circ$. Derive the equations of motion using calculus and determine the flight parameters.

## Theory
We define a Cartesian coordinate system where the origin $(0,0)$ is the launch point. The only force acting is gravity $\vec{F} = -mg\hat{j}$. 

The initial velocity vector is decomposed as:

$$
\vec{v}_0 = \begin{pmatrix} v_0 \cos\theta \\ v_0 \sin\theta \end{pmatrix}
$$

## Step-by-Step Solution: Calculus Derivation

### 1. Horizontal Motion ($x$-direction)
From Newton's Second Law, $F_x = m a_x$. Since there is no air resistance, $F_x = 0$.

**Step A: Differential Equation**

$$
m \frac{d^2x}{dt^2} = 0 \implies \frac{dv_x}{dt} = 0
$$

**Step B: Integration for Velocity**
Integrate both sides with respect to $t$:

$$
\int \frac{dv_x}{dt} dt = \int 0 dt \implies v_x(t) = C_1
$$

Using initial condition $v_x(0) = v_0 \cos\theta$, we find $C_1 = v_0 \cos\theta$.

**Step C: Integration for Position**
Since $v_x = \frac{dx}{dt}$:

$$
\int \frac{dx}{dt} dt = \int v_0 \cos\theta dt \implies x(t) = (v_0 \cos\theta)t + C_2
$$

Using $x(0) = 0$, we find $C_2 = 0$.

### 2. Vertical Motion ($y$-direction)
From Newton's Second Law, $F_y = -mg$.

**Step A: Differential Equation**

$$
m \frac{d^2y}{dt^2} = -mg \implies \frac{dv_y}{dt} = -g
$$

**Step B: Integration for Velocity**

$$
\int dv_y = \int -g dt \implies v_y(t) = -gt + C_3
$$

Using initial condition $v_y(0) = v_0 \sin\theta$, we find $C_3 = v_0 \sin\theta$:

$$
v_y(t) = v_0 \sin\theta - gt
$$

**Step C: Integration for Position**
Since $v_y = \frac{dy}{dt}$:

$$
\int dy = \int (v_0 \sin\theta - gt) dt \implies y(t) = (v_0 \sin\theta)t - \frac{1}{2}gt^2 + C_4
$$

Using $y(0) = 0$, we find $C_4 = 0$.



### 2. Time of Flight
The projectile hits the ground when $y(t) = 0$ for $t > 0$:

$$
0 = t(v_0 \sin\theta - \frac{1}{2}gt)
$$

$$
t_f = \frac{2v_0 \sin\theta}{g}
$$

Using $v_0 = 100$, $\theta = 37^\circ$, and $g \approx 9.81 \text{ m/s}^2$:

$$
t_f = \frac{2 \cdot 100 \cdot \sin(37^\circ)}{9.81} \approx 12.27 \text{ s}
$$

### 3. Maximum Height
Maximum height occurs when $v_y(t) = 0$, which is at $t = \frac{t_f}{2}$:

$$
H = y\left(\frac{v_0 \sin\theta}{g}\right) = \frac{v_0^2 \sin^2\theta}{2g}
$$

$$
H = \frac{100^2 \cdot \sin^2(37^\circ)}{2 \cdot 9.81} \approx 184.6 \text{ m}
$$

### 4. Range
The range is the horizontal displacement at $t = t_f$:

$$
R = x(t_f) = (v_0 \cos\theta) \left(\frac{2v_0 \sin\theta}{g}\right) = \frac{v_0^2 \sin(2\theta)}{g}
$$

$$
R = \frac{100^2 \cdot \sin(74^\circ)}{9.81} \approx 979.9 \text{ m}
$$

## Final Result
* **Equations:** $\ddot{x}=0, \ddot{y}=-g$
* **Time of Flight:** $12.27 \text{ s}$
* **Max Height:** $184.6 \text{ m}$
* **Range:** $979.9 \text{ m}$

## Interpretation
The motion is parabolic. The horizontal velocity remains constant throughout the flight, while the vertical velocity changes linearly due to gravity.