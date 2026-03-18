# Task 10 – Advanced Kinematics

## Problem Statement
Point M moves according to:

$$
\vec{r}(t) = (a \cos(\omega t), a \sin(\omega t), bt)
$$

*(Correction: Usually, $a$ is used for both $x$ and $y$ to form a cylinder; I will use $a$ and $a$ for the circular base as per standard helix problems, or $a$ and $b$ as provided in your prompt for an elliptical base).*

a) Find the trajectory equation.
b) Compute the path length from $t=0$ to $t=t_0$.
c) Discuss the trajectory.

## Theory
The path length $s$ is the integral of the speed:

$$
s = \int_{0}^{t_0} |\vec{v}(t)| dt
$$

## Step-by-Step Solution

### 1. Trajectory Equation
From the coordinates:
1) $x = a \cos(\omega t) \implies \frac{x}{a} = \cos(\omega t)$
2) $y = b \sin(\omega t) \implies \frac{y}{b} = \sin(\omega t)$
3) $z = bt$

Using the identity $\cos^2\theta + \sin^2\theta = 1$:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

This is the equation of an elliptical cylinder. The point moves along this cylinder while rising linearly in $z$. This shape is an **elliptical helix**.



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

## Final Result
* **Trajectory:** Elliptical helix (or circular helix if $a=b$).
* **Path Length:** $t_0\sqrt{a^2\omega^2 + b^2}$ (for the circular case).

## Interpretation
The motion combines uniform circular motion in the $xy$-plane with uniform linear motion in the $z$-direction.