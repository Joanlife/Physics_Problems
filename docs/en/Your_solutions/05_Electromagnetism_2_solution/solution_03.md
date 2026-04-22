# Task 03 – Biot-Savart Law

## Problem Statement

A small segment of a line wire of length $\Delta L = 0.1 \text{ m}$ carries a current of $I = 3 \text{ A}$. The segment is located at a distance $r = 0.2 \text{ m}$ from a point $P$. Calculate the magnetic field $B$ at point $P$ due to this segment, assuming the segment is perpendicular to the line connecting it to $P$.

## Theory


In magnitude, where the segment is perpendicular to the radius vector ($\theta = 90^\circ$, so $\sin \theta = 1$):

$$
B \approx \frac{\mu_0}{4\pi} \frac{I \Delta L \sin \theta }{r^2}
$$

$$
B \approx \frac{\mu_0}{4\pi} \frac{I \Delta L \ }{r^2}
$$

## Step-by-Step Solution

### 1. Identify Constants and Variables
- $\mu_0 = 4\pi \times 10^{-7} \text{ T} \cdot \text{m/A}$ is the permeability of free space.
- $\mu_0 / 4\pi = 10^{-7} \text{ T} \cdot \text{m/A}$
- $I = 3 \text{ A}$
- $\Delta L = 0.1 \text{ m}$
- $r = 0.2 \text{ m}$

### 2. Set up the Calculation
Using the simplified magnitude formula:

$$
B = 10^{-7} \times \frac{3 \times 0.1}{(0.2)^2}
$$

### 3. Compute the Values
$$
B = 10^{-7} \times \frac{0.3}{0.04}
$$

$$
B = 10^{-7} \times 7.5 = 7.5 \times 10^{-7} \text{ T}
$$

## Final Result

The magnetic field at point $P$ is:

$$
B =  7.5 \times 10^{-7} \text{  T}
$$

## Interpretation

This calculation treats the wire as a "current element." Because the distance $r$ is only twice the length of the segment $\Delta L$, this is an approximation. In a real-world scenario with a long wire, we would integrate this formula along the entire length of the conductor.