# Task 08 – Work of a Variable Force

## Problem Statement

Given a one-dimensional force $F(x) = -kx$:
1. Write and solve the equation of motion.
2. Calculate the work done during displacement from $0$ to $x_0$.
3. Interpret the result as potential energy.
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Draw the graph of $F(x)$ and $U(x)$.

## Theory

Work done by a variable force is the integral of the force over the displacement:

$$
W = \int_{x_1}^{x_2} F(x) dx
$$

The change in potential energy is defined as the negative of the work done by a conservative force: $\Delta U = -W$.

## Step-by-Step Solution

### 1. Equation of Motion

From $F = ma$:

$$
m \frac{d^2x}{dt^2} = -kx \implies \frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

This is a second-order linear differential equation. The general solution is:

$$
x(t) = A \cos(\omega t + \phi), \quad \omega = \sqrt{\frac{k}{m}}
$$

### 2. Work Calculation

$$
W = \int_{0}^{x_0} (-kx) dx = -k \left[ \frac{1}{2}x^2 \right]_0^{x_0} = -\frac{1}{2}kx_0^2
$$

### 3. Potential Energy Interpretation

Since $W = -\Delta U$ and assuming $U(0) = 0$:

$$
U(x_0) = -W = \frac{1}{2}kx_0^2
$$

This represents the elastic potential energy stored in the system.

### 4. Verification

$$
-\frac{dU}{dx} = -\frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = -k \cdot x = F(x)
$$

The relationship holds.

## Final Result

* Work: $W = -\frac{1}{2}kx_0^2$
* Potential Energy: $U(x) = \frac{1}{2}kx^2$

## Interpretation

The negative work indicates that the force is "restoring"—it acts in the opposite direction of the displacement. The potential energy is parabolic, meaning the energy grows quadratically as the displacement increases from equilibrium.