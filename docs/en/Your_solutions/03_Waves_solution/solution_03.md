# Task 03 – Superposition Principle

## Problem Statement

Two waves are described by the equations $y_1(x, t) = A \sin(kx - \omega t)$ and $y_2(x, t) = A \sin(kx + \omega t)$. What is the equation of the resulting standing wave? Identify the positions of the nodes.

## Theory

The principle of superposition states that the resultant displacement of two overlapping waves is the algebraic sum of their individual displacements:

$$
y_{res}(x, t) = y_1(x, t) + y_2(x, t)
$$

To simplify the sum of two sine functions, we use the trigonometric identity:

$$
\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)
$$

## Step-by-Step Solution

### 1. Derivation of the Standing Wave Equation
Let $\alpha = kx - \omega t$ and $\beta = kx + \omega t$.

$$
y_{res} = A [\sin(kx - \omega t) + \sin(kx + \omega t)]
$$

Applying the identity:

$$
y_{res} = A \left[ 2 \sin\left(\frac{(kx - \omega t) + (kx + \omega t)}{2}\right) \cos\left(\frac{(kx - \omega t) - (kx + \omega t)}{2}\right) \right]
$$

Simplifying the arguments:

$$
y_{res} = 2A \sin(kx) \cos(-\omega t)
$$

Since cosine is an even function, $\cos(-\omega t) = \cos(\omega t)$:

$$
y_{res}(x, t) = [2A \sin(kx)] \cos(\omega t)
$$

### 2. Identifying Node Positions
Nodes are points where the displacement is always zero ($y_{res} = 0$) regardless of time $t$. This occurs when the spatial part of the equation is zero:

$$
\sin(kx) = 0
$$

This condition is satisfied when the argument $kx$ is an integer multiple of $\pi$:

$$
kx = n\pi, \quad n = 0, \pm 1, \pm 2, \dots
$$

Since the wave number $k$ is defined as $k = \frac{2\pi}{\lambda}$, we substitute:

$$
\left(\frac{2\pi}{\lambda}\right) x = n\pi
$$

Solving for $x$:

$$
x = \frac{n\lambda}{2}
$$

## Final Result

The equation of the standing wave is:

$$
y(x, t) = 2A \sin(kx) \cos(\omega t)
$$

The nodes are located at:

$$
x = n \frac{\lambda}{2} \quad \text{for } n \in \mathbb{Z}
$$

## Interpretation

The resulting equation separates the spatial dependency $\sin(kx)$ from the temporal dependency $\cos(\omega t)$. Unlike a traveling wave, the positions of the peaks (antinodes) and zeros (nodes) do not move through space; only the local amplitude oscillates in time.