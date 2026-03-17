# Task 04 – Vector Calculus

## Problem Statement

The position vector is

$$
\vec r(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}
$$

Find velocity and acceleration.

---

## Theory

Velocity is the derivative of position.

$$
\vec v(t) = \frac{d\vec r}{dt}
$$

Acceleration is the derivative of velocity.

$$
\vec a(t) = \frac{d\vec v}{dt}
$$

---

## Step-by-Step Solution

### Velocity

Differentiate each component.

$$
v_x = \frac{d}{dt}(3t^2) = 6t
$$

$$
v_y = \frac{d}{dt}(5t - 8t^2) = 5 - 16t
$$

Thus

$$
\vec v(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

---

### Acceleration

Differentiate velocity.

$$
a_x = 6
$$

$$
a_y = -16
$$

Therefore

$$
\vec a(t) = 6\hat{i} -16\hat{j}
$$

---

## Final Result

Velocity:

$$
\vec v(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

Acceleration:

$$
\vec a(t) = 6\hat{i} -16\hat{j}
$$

---

## Interpretation

The acceleration is constant since in the final acceleration vector has no t in it, which indicates uniformly accelerated motion meaning the acceleration does not change as time passes.