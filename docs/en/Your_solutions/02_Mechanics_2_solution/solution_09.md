# Task 09 – Vertical Throw with Drag

## Problem Statement

Equation of motion: $m \frac{dv}{dt} = -mg - kv$ with $v(0) = v_0$ and $x(0) = 10$.
1. Solve analytically for $v(t)$.
2. Determine maximum height.
3. Compare with the vacuum case ($k=0$).

## Theory

This is a first-order linear differential equation. The term $-kv$ represents linear air resistance (Stokes' drag), which depends on the velocity of the object.

## Step-by-Step Solution

### 1. Analytical Solution for Velocity

Rearrange the equation. First,divide by m:


$$
\frac{dv}{dt} = -\left( g + \frac{k}{m}v \right)
$$

Separate variables:

$$
\int \frac{dv}{g + \frac{k}{m}v} = -\int dt
$$

Integrating both sides:

$$
\frac{m}{k} \ln\left( g + \frac{k}{m}v \right) = -t + C
$$

Applying $v(0) = v_0$: $C = \frac{m}{k} \ln(g + \frac{k}{m}v_0)$. Solving for $v(t)$:

$$
v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}
$$

### 2. Maximum Height

At $h_{max}$, $v(t) = 0$. Solve for $t_{rise}$:

$$
0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{rise}} - \frac{mg}{k} \implies e^{-\frac{k}{m}t_{rise}} = \frac{mg}{kv_0 + mg}
$$

Integrating $v(t)$ from $0$ to $t_{rise}$ and adding initial height $x(0) = 10$ gives $x_{max}$.

### 3. Comparison

In a vacuum ($k=0$):
* $h_{max} = x(0) + \frac{v_0^2}{2g}$
* $v(t) = v_0 - gt$

With drag, $h_{max}$ is strictly lower because energy is dissipated as heat throughout the ascent.

## Final Result

The velocity decays exponentially toward a terminal velocity $v_t = -\frac{mg}{k}$.

## Interpretation

Unlike the vacuum case where acceleration is constant, here acceleration decreases as the object slows down (during ascent) and would eventually reach a balance point if falling.