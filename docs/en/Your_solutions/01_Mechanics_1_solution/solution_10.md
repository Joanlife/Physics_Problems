# Task 10 – Kinematics in 3D

## Problem Statement

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

Determine:

- trajectory
- path length
- visualize motion

---

## Theory

The motion combines:

- circular motion in $xy$
- linear motion in $z$

This creates a **helix**.

---

## Step-by-Step Solution

### Trajectory
From the coordinates,we rearrange these to:
1) $x = a \cos(\omega t) \implies \frac{x}{a} = \cos(\omega t)$
2) $y = b \sin(\omega t) \implies \frac{y}{b} = \sin(\omega t)$
3) $z = bt$

Using the trigonometric identity $\cos^2\theta + \sin^2\theta = 1$:
From $x$ and $y$:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

This is an ellipse.

Since $z = bt$, the motion rises linearly.

Thus trajectory is a helix.

---

### 2. Path Length Calculation
First, find velocity:

$$
\vec{v}(t) = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)
$$

The speed $|\vec{v}(t)|$ is:

$$
v = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}
$$

Assuming a circular base ($a=b$):

$$
v = \sqrt{a^2\omega^2(\sin^2(\omega t) + \cos^2(\omega t)) + b^2} = \sqrt{a^2\omega^2 + b^2}
$$

Since speed is constant, the path length is:

$$
s = \int_{0}^{t_0} \sqrt{a^2\omega^2 + b^2} dt = t_0\sqrt{a^2\omega^2 + b^2}
$$


---

## Final Result
- trajectory: helix
- motion: periodic in plane, linear in height
* Path Length: $t_0\sqrt{a^2\omega^2 + b^2}$ (for the circular case).


---

