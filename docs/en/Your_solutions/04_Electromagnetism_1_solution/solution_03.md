# Task 03 – Electrostatic Equilibrium

## Problem Statement

Find the equilibrium position for a charge $q_3 = +1$ C placed on the line between a charge $q_1 = +4$ C and a charge $q_2 = +9$ C, which are separated by a distance of $2$ m.

## Theory

Equilibrium whereby $q_3$ stays perfectly still occurs when the net force on $q_3$ is zero:

$$
\vec{F}_{net} = \vec{F}_{13} + \vec{F}_{23} = 0
$$

Since $q_1, q_2,$ and $q_3$ are all positive, $q_3$ will be repelled by both $q_1$ and $q_2$. For these forces to cancel, $q_3$ must be placed between them so the forces point in opposite directions.

## Step-by-Step Solution

### 1. Define Coordinates
Let $q_1$ be at $x = 0$ and $q_2$ be at $x = 2$ m. Let $q_3$ be at position $x$.
- Distance from $q_1$ to $q_3$ is $x$.
- Distance from $q_2$ to $q_3$ is $2 - x$.

### 2. Set Up the Equation
The magnitudes of the forces must be equal:

$$
k \frac{q_1 q_3}{x^2} = k \frac{q_2 q_3}{(2 - x)^2}
$$

Divide both sides by $k q_3$:

$$
\frac{q_1}{x^2} = \frac{q_2}{(2 - x)^2}
$$

### 3. Solve for $x$
Substitute $q_1 = 4$ and $q_2 = 9$:

$$
\frac{4}{x^2} = \frac{9}{(2 - x)^2}
$$

Take the square root of both sides:

$$
\frac{2}{x} = \frac{3}{2 - x}
$$

Cross-multiply:

$$
2(2 - x) = 3x
$$

$$
4 - 2x = 3x
$$

$$
4 = 5x \implies x = 0.8 \text{ m}
$$

$$
2-x=2-0.8=1.2 m
$$

## Final Result

The equilibrium position is $0.8$ m from the charge $q_1 = +4$ C and $1.2$ m from the charge $q_2 = +9$ C.

## Interpretation

The equilibrium point is closer to the smaller charge ($q_1$) because its weaker field needs a shorter distance to produce a force equal to that of the much stronger charge ($q_2$). This is a stable equilibrium point along the x-axis for $q_3$.