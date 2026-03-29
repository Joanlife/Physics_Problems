# Task 02 – Harmonic Motion of a Spring-Mass System

## Problem Statement

A $10\text{ kg}$ mass is attached to a spring and oscillates according to the equation:

$$
x(t) = 0.2 \cos(10\pi t)
$$

Find:
1. The spring constant $k$.
2. The total mechanical energy of the system.

## Theory

The general equation for simple harmonic motion (SHM) is:

$$
x(t) = A \cos(\omega t + \phi)
$$

Where:
* $A$ is the amplitude.
* $\omega$ is the angular frequency, defined as $\omega = \sqrt{\frac{k}{m}}$.
* $k$ is the spring constant and $m$ is the mass.

The total mechanical energy $E$ in SHM is constant and given by:

$$
E = \frac{1}{2} k A^2
$$

## Step-by-Step Solution

### 1. Finding the Spring Constant

From the given equation $x(t) = 0.2 \cos(10\pi t)$, we identify:
* $A = 0.2\text{ m}$
* $\omega = 10\pi\text{ rad/s}$

Using the relation for $\omega$:

$$
\omega^2 = \frac{k}{m} \implies k = m \omega^2
$$

Substituting $m = 10\text{ kg}$ and $\omega = 10\pi$:

$$
k = 10 \cdot (10\pi)^2 = 10 \cdot 100\pi^2 = 1000\pi^2
$$

$$
k \approx 1000 \cdot 9.87 \approx 9869.6\text{ N/m}
$$

### 2. Finding Total Mechanical Energy

Using the energy formula:

$$
E = \frac{1}{2} k A^2
$$

$$
E = \frac{1}{2} (1000\pi^2) (0.2)^2
$$

$$
E = 500\pi^2 \cdot 0.04 = 20\pi^2
$$

$$
E \approx 20 \cdot 9.87 \approx 197.39\text{ J}
$$

## Final Result

* Spring constant: $k = 1000\pi^2 \approx 9870\text{ N/m}$
* Total energy: $E = 20\pi^2 \approx 197.4\text{ J}$

## Interpretation

The high spring constant indicates a very stiff spring, which is consistent with the high angular frequency of $10\pi\text{ rad/s}$ (5 oscillations per second) despite the large $10\text{ kg}$ mass.