# Task 02 – Ampere's Law

## Problem Statement

Two long, parallel wires are $d = 10 \text{ cm}$ apart and carry currents of $I = 5 \text{ A}$ in opposite directions. Calculate the magnitude and direction of the magnetic field $\mathbf{B}$ at a point $P$ midway between the wires.

## Theory

The magnetic field $B$ produced by a long, straight wire at a distance $r$ is given by:

$$
B = \frac{\mu_0 I}{2 \pi r}
$$

Where:
- $\mu_0 = 4\pi \times 10^{-7} \text{ T} \cdot \text{m/A}$ is the permeability of free space.
- $I$ is the current.
- $r$ is the perpendicular distance from the wire.

The direction of the field is determined by the **Right-Hand Rule**: point your thumb in the direction of the current, and your fingers curl in the direction of the magnetic field lines.

## Step-by-Step Solution

### 1. Determine the Distance to the Midpoint
The total distance between the wires is $d = 0.1 \text{ m}$. The midpoint $P$ is at a distance $r$ from each wire:

$$
r = \frac{d}{2} = 0.05 \text{ m}
$$

### 2. Determine Directions using Right-Hand Rule
- **Wire 1 (Current "Up"):** At the midpoint (to the right of wire 1), the field $B_1$ points into the page.
- **Wire 2 (Current "Down"):** At the midpoint (to the left of wire 2), the field $B_2$ also points into the page.

Since both vectors point in the same direction, the total magnetic field $B_{total}$ is the sum of the magnitudes.

### 3. Calculate Individual Magnitudes
Since $I_1 = I_2 = 5 \text{ A}$ and $r_1 = r_2 = 0.05 \text{ m}$:

$$
B_1 = B_2 = \frac{4\pi \times 10^{-7} \times 5}{2\pi \times 0.05}
$$

$$
B_1 = B_2 = \frac{2 \times 10^{-7} \times 5}{0.05} = 2 \times 10^{-5} \text{ T}
$$

### 4. Calculate Total Field
$$
B_{total} = B_1 + B_2 = 2 \times 10^{-5} + 2 \times 10^{-5} = 4\times 10^{-5}   \text{ T}
$$

## Final Result

The magnitude of the magnetic field at the midpoint is:

$$
B = 4 \times 10^{-5}  \text{ T}
$$

The direction is perpendicular to the plane containing the wires (into the page, assuming the "Up/Down" orientation described).

## Interpretation

In a configuration with opposite currents (anti-parallel), the magnetic fields between the wires reinforce each other. If the currents were in the same direction, the fields would cancel at the midpoint.

![alt text](<diagram 2.jpeg>)