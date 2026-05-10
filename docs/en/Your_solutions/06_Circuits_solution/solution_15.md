# Task 15 – Resistor Cube

## Problem Statement

A cube is constructed from 12 identical resistors, each of resistance $R$. What is the equivalent resistance ($R_{eq}$) between two opposite corners (the body diagonal)?

## Theory



This problem is best solved using **symmetry and potential distribution**. If we apply a voltage $V$ across opposite corners, the current must distribute itself according to the symmetry of the cube.

## Step-by-Step Solution

### 1. Current Distribution
Let a total current $I$ enter at corner $A$ and leave at the opposite corner $G$.
- At corner $A$, the current splits into **3 equal edges**. Current per edge = $I/3$.
- Each of those 3 edges leads to a junction where the current splits into **2 more edges**. Current per edge = $(I/3) / 2 = I/6$.
- Finally, these currents recombine at the last 3 edges leading to corner $G$. Current per edge = $I/3$.

### 2. Voltage Drop Calculation
The total voltage drop $V$ across the body diagonal is the sum of voltage drops along any path from $A$ to $G$. Let's take one path:

$$
\begin{align}
V &= V_{edge1} + V_{edge2} + V_{edge3} \\
  &= \left(\frac{I}{3}\right)R + \left(\frac{I}{6}\right)R + \left(\frac{I}{3}\right)R
\end{align}
$$

### 3. Finding Equivalent Resistance
Combine the fractions:

$$
\begin{align}
V &= IR \left( \frac{2}{6} + \frac{1}{6} + \frac{2}{6} \right) \\
V &= IR \left( \frac{5}{6} \right)
\end{align}
$$

Using $R_{eq} = \frac{V}{I}$:

$$
R_{eq} = \frac{5}{6}R
$$

## Final Result

$$
R_{eq} = \frac{5}{6}R
$$

## Interpretation
Due to the highly symmetrical nature of the cube, we can treat nodes of equal potential as being connected. This simplifies the 12-resistor network into a series combination of three parallel groups ($3 \parallel 6 \parallel 3$).