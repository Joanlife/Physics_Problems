# Task 01 – Propagation of Error I

## Problem Statement
The radius of a sphere is measured to be $r = (6.20 \pm 0.05)\text{ cm}$. Calculate the volume of the sphere and its associated uncertainty.

## Theory
The volume of a sphere is given by the geometric formula:

$$
V = \frac{4}{3} \pi r^3
$$

For a physical quantity defined by a power law $V \propto r^3$, the relative uncertainty is found by multiplying the exponent by the relative uncertainty of the base variable:

$$
\frac{\Delta V}{V} = 3 \frac{\Delta r}{r}
$$

## Step-by-Step Solution
First, compute the central value for the volume based on the measured radius:

$$
\begin{align}
V &= \frac{4}{3} \pi (6.20)^3 \\
  &\approx \frac{4}{3} \pi (238.328) \\
  &\approx 998.31 \text{ cm}^3
\end{align}
$$

Next, determine the absolute uncertainty $\Delta V$ using the relative uncertainty formula:

$$
\begin{align}
\Delta V &= V \left( 3 \frac{\Delta r}{r} \right) \\
         &= 998.31 \left( 3 \frac{0.05}{6.20} \right) \\
         &= 998.31 (0.02419) \\
         &\approx 24.15 \text{ cm}^3
\end{align}
$$

Rounding the uncertainty to two significant figures yields $\Delta V \approx 24 \text{ cm}^3$. The volume is rounded to match this decimal precision.

## Final Result

$$
V = (998 \pm 24) \text{ cm}^3
$$

## Interpretation
The volume of the sphere is approximately $998 \text{ cm}^3$. The measurement uncertainty of $0.05 \text{ cm}$ in the radius expands to an uncertainty of roughly $24 \text{ cm}^3$ in the volume. This demonstrates how cubic relationships magnify small measurement errors.