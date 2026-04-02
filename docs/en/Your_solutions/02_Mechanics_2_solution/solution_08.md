# Task 08 – Work of a Variable Force

## Problem Statement

Given a one-dimensional force $F(x) = -kx$:
1. Write down the equation of motion and solve it.
2. Calculate the work done during the displacement from $0$ to $x_0$.
3. Interpret the result as potential energy.
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Draw the graph of $F(x)$ and $U(x)$.

## Theory

When a force depends on position, such as a spring force, we cannot simply multiply force by distance ($W = Fd$) because the force value changes at every point. Instead, we must use **integration**, which sums up the "infinitesimal" work done over tiny slices of distance $dx$.

$$
W = \int_{x_{start}}^{x_{end}} F(x) dx
$$

In a conservative field, the work done by the field reduces the system's potential energy ($W = -\Delta U$).

## Step-by-Step Solution

### 1. Equation of Motion
Applying Newton's Second Law ($F = ma$):

$$
m \frac{d^2x}{dt^2} = -kx
$$

To solve this, we rewrite it as a standard harmonic oscillator equation:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

The solution is a sinusoidal function, representing periodic back-and-forth motion:

$$
x(t) = A \cos(\omega t + \phi), \quad \text{where } \omega = \sqrt{\frac{k}{m}}
$$

### 2. Calculating Work (The "Summing" Method)
We calculate the work done by the force $F(x) = -kx$ as the object moves from $0$ to $x_0$:

$$
W = \int_{0}^{x_0} (-kx) dx
$$

Using the power rule for integration ($\int x^n dx = \frac{x^{n+1}}{n+1}$):

$$
W = -k \left[ \frac{1}{2}x^2 \right]_{0}^{x_0}
$$

$$
W = -k \left( \frac{1}{2}x_0^2 - \frac{1}{2}(0)^2 \right) = -\frac{1}{2}kx_0^2
$$

### 3. Potential Energy Interpretation
Potential energy ($U$) is defined as the capacity to do work. Because the force $-kx$ is "conservative," the work done *against* the force is stored as potential energy.

$$
\Delta U = -W = \frac{1}{2}kx_0^2
$$

Assuming the energy is zero at the equilibrium point ($x=0$), the potential energy function is:

$$
U(x) = \frac{1}{2}kx^2
$$

### 4. Verification of $F = -\frac{dU}{dx}$
We verify that the force is the negative gradient (slope) of the potential energy:

$$
-\frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = -\left( \frac{1}{2} \cdot k \cdot 2x \right) = -kx
$$

The derivative confirms that the force $F(x)$ always points "downhill" toward the minimum potential energy.
![Graph of force F(x)=-kx and potential energy U(x)=½kx² over position x. The force is a linear downward slope, and the energy is a positive parabola, highlighting their derivative relationship.](graph%20no%208.jpeg)

## Final Result

* **Work Done by Force:** $W = -\frac{1}{2}kx_0^2$
* **Potential Energy:** $U(x) = \frac{1}{2}kx^2$
* **Force Relation:** $F = -kx$

## Interpretation



The graph of $F(x)$ is a straight line with a negative slope, showing that the further you pull the object, the harder it pulls back. The graph of $U(x)$ is a **parabola**. This "potential well" explains why objects oscillate: they are always being pushed back toward the bottom of the $U(x)$ curve.