# Task 03 – Conservation of Energy in a Pendulum

## Problem Statement

A pendulum with a length of $1.0\text{ m}$ is released from an initial angle of $15^\circ$. What is the speed of the pendulum bob at the bottom of its swing?

## Theory

In a frictionless system, the total mechanical energy is conserved:

$$
E_{top} = E_{bottom}
$$

At the release point (top), the bob has only gravitational potential energy ($U$). At the lowest point (bottom), this is converted entirely into kinetic energy ($K$).

The height $h$ relative to the bottom is:

$$
h = L - L \cos(\theta) = L(1 - \cos\theta)
$$

## Step-by-Step Solution

### 1. Energy Balance Equation

$$
mgh = \frac{1}{2} mv^2
$$

The mass $m$ cancels out:

$$
gh = \frac{1}{2} v^2 \implies v = \sqrt{2gh}
$$

### 2. Calculate the Height

Given $L = 1.0\text{ m}$ and $\theta = 15^\circ$:

$$
h = 1.0 \cdot (1 - \cos(15^\circ))
$$

Using $\cos(15^\circ) \approx 0.9659$:

$$
h = 1.0 \cdot (1 - 0.9659) = 0.0341\text{ m}
$$

### 3. Calculate the Velocity

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

$$
v = \sqrt{0.669} \approx 0.818\text{ m/s}
$$

## Final Result

The speed of the bob at the bottom of the swing is approximately $0.82\text{ m/s}$.              



## Interpretation

The speed depends only on the vertical drop $h$, not on the mass of the bob. Since $15^\circ$ is a relatively small angle, the vertical displacement is small ($3.4\text{ cm}$), resulting in a modest velocity at the equilibrium point.
![Diagram of a pendulum showing the relationship between string length L, angle theta, and height h.](Bob%20illustration.jpeg)