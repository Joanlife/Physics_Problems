# Task 06 – Wave Equation Analysis

## Problem Statement

A wave is described by the equation $y(x,t) = 0.05 \sin(2\pi x - 50\pi t)$, where $x$ and $y$ are in meters and $t$ is in seconds. Determine:
a) Amplitude $A$
b) Wavelength $\lambda$
c) Frequency $f$
d) Wave speed $v$

## Theory

The standard form of a harmonic traveling wave is:

$$
y(x,t) = A \sin(kx - \omega t)
$$

By comparing the given equation to the standard form, we can extract:
* **Amplitude ($A$):** The coefficient in front of the sine.
* **Wave number ($k$):** The coefficient of $x$, where $k = \frac{2\pi}{\lambda}$.
* **Angular frequency ($\omega$):** The coefficient of $t$, where $\omega = 2\pi f$.

## Step-by-Step Solution

The given equation is:

$$
y(x,t) = 0.05 \sin(2\pi x - 50\pi t)
$$

### a) Amplitude $A$
Direct comparison yields:

$$
A = 0.05 \text{ m}
$$

### b) Wavelength $\lambda$
From the equation, $k = 2\pi \text{ rad/m}$.
Using the definition $k = \frac{2\pi}{\lambda}$:

$$
2\pi = \frac{2\pi}{\lambda} \implies \lambda = 1 \text{ m}
$$

### c) Frequency $f$
From the equation, $\omega = 50\pi \text{ rad/s}$.
Using the definition $\omega = 2\pi f$:

$$
50\pi = 2\pi f \implies f = 25 \text{ Hz}
$$

### d) Wave speed $v$
The wave speed can be calculated using $v = f\lambda$ or $v = \frac{\omega}{k}$:

$$
v = 25 \text{ Hz} \times 1 \text{ m} = 25 \text{ m/s}
$$

## Final Result

* **Amplitude:** $0.05 \text{ m}$
* **Wavelength:** $1 \text{ m}$
* **Frequency:** $25 \text{ Hz}$
* **Wave speed:** $25 \text{ m/s}$

## Interpretation

The wave is traveling in the positive x-direction (indicated by the minus sign between the $kx$ and $\omega t$ terms). It oscillates 25 times per second and repeats its spatial pattern every 1 meter.