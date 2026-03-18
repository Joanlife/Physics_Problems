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

## Step-by-Step Solution: Calculus Derivation

### 1. Horizontal Motion ($x$-direction)
From Newton's Second Law, $F_x = m a_x$. Since there is no air resistance, $F_x = 0$ and since acceleration is the second derivative of velocity $$a_x = \frac{d^2x}{dt^2}$$

**Calculating Differential Equation**

$$
m \frac{d^2x}{dt^2} = 0 \implies \frac{dv_x}{dt} = 0
$$



### 2. Vertical Motion ($y$-direction)
From Newton's Second Law, $F_y = -mg$, $$a_y = \frac{d^2y}{dt^2}$$

**Calculating Differential Equation**

$$
m \frac{d^2y}{dt^2} = -mg \implies \frac{dv_y}{dt} = -g
$$


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