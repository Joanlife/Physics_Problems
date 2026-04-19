# Task 06 – EM Wave Analysis

## Problem Statement

An electromagnetic wave has its Electric field component by: $E_y(x,t) = 100 \sin(10^7 x - \omega t) \text{ V/m}$. Find direction of propagation, wavelength $\lambda$, angular frequency $\omega$, and the equation for the magnetic field component.

## Theory

A general harmonic EM wave is described by:

$$
E = E_0 \sin(kx - \omega t)
$$

Where:
- $k$ is the wave number ($k = 2\pi / \lambda$).
- $\omega$ is the angular frequency ($\omega = 2\pi f = ck$).
- $c$ is the speed of light ($3 \times 10^8 \text{ m/s}$).
- $E_0$ is the amplitude

## Step-by-Step Solution

### 1. Direction of Propagation
The argument of the sine function is $(kx - \omega t)$. Since the sign between the spatial part ($x$) and temporal part ($t$) is negative, the wave propagates in the **positive x-direction**.

### 2. Wavelength ($\lambda$)
From the equation, $k = 10^7 \text{ rad/m}$.

$$
\lambda = \frac{2\pi}{k} = \frac{2\pi}{10^7} \approx 6.28 \times 10^{-7} \text{ m} = 628 \text{ nm}
$$

### 3. Angular Frequency ($\omega$)
$$
\omega = c \cdot k = (3 \times 10^8) \times 10^7 = 3 \times 10^{15} \text{ rad/s}
$$

### 4. Magnetic Field Equation
The magnetic field $B$ is perpendicular to $E$ and the direction of propagation. Since $E$ is in the $y$ direction and propagation is in $x$, $B$ must be in the $z$ direction.

Magnitude $B_0$:
$$
B_0 = \frac{E_0}{c} = \frac{100}{3 \times 10^8} \approx 3.33 \times 10^{-7} \text{ T}
$$

The phase remains the same:
$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t) \text{ T}
$$

## Final Result

- Direction: $+x$
- $\lambda \approx 628 \text{ nm}$
- $\omega = 3 \times 10^{15} \text{ rad/s}$
- $B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t) \text{ T}$

## Interpretation

This wave is in the visible spectrum (reddish light). The extremely high frequency and small wavelength are typical for light waves.