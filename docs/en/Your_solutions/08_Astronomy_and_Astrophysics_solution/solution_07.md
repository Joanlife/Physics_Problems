# Task 07 – Megastructures

## Problem Statement

A "Dyson Sphere" is a hypothetical megastructure that completely encompasses a star to capture its entire energy output. If the mass of Mercury ($M_{\text{Merc}} \approx 3.3 \times 10^{23}$ kg) were completely dismantled and repurposed to build a uniform solid solar panel sphere with a surface density of $\sigma = 10$ kg/m², what would be the resulting radius of this megastructure?

## Theory

The concept depends on the distribution of a finite total mass $M$ evenly over a spherical shell area. The surface mass density $\sigma$ relates the total mass to the area $A$ of the shell via the definition

$$
\sigma = \frac{M}{A}
$$

The area of a perfect sphere with radius $r$ is formulated as

$$
A = 4\pi r^2
$$

Combining these two expressions yields a direct connection between material constraints and structural geometry

$$
\sigma = \frac{M}{4\pi r^2}
$$

Isolating the structural radius $r$ yields the equation

$$
r^2 = \frac{M}{4\pi \sigma} \implies r = \sqrt{\frac{M}{4\pi \sigma}}
$$

## Step-by-Step Solution

Extract the mathematical parameters from the structural statement

$$
M = 3.3 \times 10^{23}\,\text{kg}
$$

$$
\sigma = 10\,\text{kg/m}^2
$$

Substitute the variables into the isolated geometric formula

$$
r = \sqrt{\frac{3.3 \times 10^{23}}{4 \pi \times 10}}
$$

Simplify the denominator inside the radical

$$
4 \pi \times 10 = 40\pi \approx 125.6637\,\text{kg/m}^2
$$

Perform the internal division step

$$
\frac{3.3 \times 10^{23}}{125.6637} \approx 2.62606 \times 10^{21}\,\text{m}^2
$$

Extract the square root to find the radius dimensions

$$
r = \sqrt{2.62606 \times 10^{21}} \approx 5.1245 \times 10^{10}\,\text{m}
$$

Convert the final unit scale into millions of kilometers to compare with standard astronomical lengths

$$
r \approx 51.25 \times 10^6\,\text{km}
$$

## Final Result

The radius of the constructed Dyson Sphere would be approximately $5.12 \times 10^{10}\,\text{m}$, or $51.2\,\text{million kilometers}$.

## Interpretation

To understand the scale of this megastructure, it helps to compare it to the real solar system. The average distance from Mercury to the Sun is about $57.9 \times 10^6\,\text{km}$. This means that the mass of Mercury is sufficient to build a thin shell enclosing the Sun that sits entirely inside Mercury's original orbit (at roughly $0.34\,\text{Astronomical Units}$). This calculation shows that engineering a stellar energy collector is theoretically possible using the material resources already available in the inner solar system.