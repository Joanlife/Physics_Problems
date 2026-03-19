# Task 10 – Infinite Series (The Ant's Path)

## Problem Statement
An ant moves 1 m East, 1/2 m North, 1/3 m West, 1/4 m South, 1/5 m East, etc. Determine its final position $(x, y)$.

## Theory
The movement follows the alternating harmonic series in two separate dimensions.
East/West moves affect $x$: $1 - 1/3 + 1/5 - 1/7 \dots$
North/South moves affect $y$: $1/2 - 1/4 + 1/6 - 1/8 \dots$

## Step-by-Step Solution

### X-Coordinate
Horizontal displacement:

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots
$$
The series is the expansion for $\arctan(x)$ where $x=1$:

$$
x = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1} = \frac{\pi}{4}
$$

### Y-Coordinate
Vertical displacement:

$$
\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots
$$
The series is half of the alternating harmonic series $\ln(2)$:

$$
y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} \dots = \frac{1}{2} \left( 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} \dots \right)
$$

$$
y = \frac{1}{2} \ln(2)
$$

## Final Result
The final position is $\left( \frac{\pi}{4}, \frac{\ln(2)}{2} \right)$.

## Interpretation
The ant's path spirals inward toward a specific limit point, demonstrating how discrete steps can converge to a coordinate defined by transcendental numbers.