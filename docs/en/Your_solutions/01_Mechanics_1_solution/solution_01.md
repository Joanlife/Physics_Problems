# Solutions goes here

# Task 01 – Projectile Motion

## Problem Statement

A projectile is fired from the ground with an initial velocity of $100 \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Air resistance is neglected.

Determine:

- the differential equations of motion
- the time of flight
- the maximum height
- the range

---

## Theory

Projectile motion under constant gravitational acceleration is described by Newton's second law.

Only gravity acts on the projectile:

$$
\vec{F} = m\vec{a}
$$

The gravitational acceleration is

$$
\vec{a} = (0,-g)
$$

where

$$
g \approx 9.81 \text{ m/s}^2
$$

The motion separates naturally into horizontal and vertical components.

---

## Step-by-Step Solution

### Initial Velocity Components

The initial velocity $v_0$ is decomposed into components:

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

For

$$
v_0 = 100
$$

$$
\theta = 37^\circ
$$

Approximate values:

$$
v_{0x} \approx 100 \cos 37^\circ \approx 80
$$

$$
v_{0y} \approx 100 \sin 37^\circ \approx 60
$$

---

### Differential Equations of Motion

Horizontal direction:

$$
\frac{d^2 x}{dt^2} = 0
$$

Vertical direction:

$$
\frac{d^2 y}{dt^2} = -g
$$

---

### Velocity Functions

Integrating acceleration gives velocity.

Horizontal velocity:

$$
v_x(t) = v_{0x}
$$

Vertical velocity:

$$
v_y(t) = v_{0y} - gt
$$

---

### Position Functions

Integrating velocity:

$$
x(t) = v_{0x} t
$$

$$
y(t) = v_{0y} t - \frac{1}{2}gt^2
$$

---

### Time of Flight

The projectile lands when

$$
y(T) = 0
$$

Thus

$$
0 = v_{0y}T - \frac{1}{2}gT^2
$$

Factor:

$$
T(v_{0y} - \frac{gT}{2}) = 0
$$

Non-trivial solution:

$$
T = \frac{2v_{0y}}{g}
$$

Substitute values:

$$
T = \frac{2(60)}{9.81}
$$

$$
T \approx 12.2 \text{ s}
$$

---

### Maximum Height

Maximum height occurs when

$$
v_y = 0
$$

Thus

$$
0 = v_{0y} - gt
$$

$$
t = \frac{v_{0y}}{g}
$$

Substitute into the position equation:

$$
H = \frac{v_{0y}^2}{2g}
$$

Numerically:

$$
H = \frac{60^2}{2(9.81)}
$$

$$
H \approx 183.5 \text{ m}
$$

---

### Range

The horizontal range is

$$
R = v_{0x}T
$$

Substitute values:

$$
R = 80 \times 12.2
$$

$$
R \approx 976 \text{ m}
$$

---

## Final Result

Time of flight:

$$
T \approx 12.2 \text{ s}
$$

Maximum height:

$$
H \approx 183.5 \text{ m}
$$

Range:

$$
R \approx 976 \text{ m}
$$

---

## Interpretation

The horizontal and vertical motions are independent.

Gravity affects only the vertical motion, while horizontal velocity remains constant. The resulting trajectory is a parabola....