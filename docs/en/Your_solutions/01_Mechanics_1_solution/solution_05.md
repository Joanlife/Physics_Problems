# Task 05 – Relative Velocity

## Problem Statement
A river flows east at $v_r = 2 \text{ m/s}$. A boat moves at $v_b = 5 \text{ m/s}$ in still water. The boat wants to travel directly north across a river 200 meters wide.
* Determine the heading angle $\theta$.
* Determine the crossing time $t$.

## Theory
This is a relative velocity problem simply because of the "cross-current" interaction since the problem states the boat wants to travel "directly north" while the river flows "east". Let $\vec{v}_{br}$ be the velocity of the boat relative to the river, $\vec{v}_r$ the velocity of the river relative to the ground, and $\vec{v}_{bg}$ the velocity of the boat relative to the ground.

$$
\vec{v}_{bg} = \vec{v}_{br} + \vec{v}_r
$$

For the boat to travel directly north, the eastward component of its velocity relative to the ground must be zero.



## Step-by-Step Solution

### 1. Finding the Heading Angle
Let the angle $\theta$ be measured from the North direction toward the West (upstream).
* River velocity: $\vec{v}_r = (2, 0)$
* Boat velocity relative to water: $\vec{v}_{br} = (-5\sin\theta, 5\cos\theta)$

For the resultant velocity $\vec{v}_{bg}$ to be purely North:

$$
v_{bg, x} = 0 \implies -5\sin\theta + 2 = 0
$$

$$
\sin\theta = \frac{2}{5} = 0.4
$$

$$
\theta = \arcsin(0.4) \approx 23.58^\circ
$$

The boat must head $23.58^\circ$ West of North.

### 2. Finding the Crossing Time
The northward velocity component determines the crossing time:

$$
v_{bg, y} = 5\cos\theta = 5\cos(23.58^\circ)
$$

$$
v_{bg, y} = 5 \sqrt{1 - \sin^2\theta} = 5 \sqrt{1 - 0.4^2} = 5 \sqrt{0.84} \approx 4.58 \text{ m/s}
$$

Using $d = v \cdot t$:

$$
t = \frac{200 \text{ m}}{4.58 \text{ m/s}} \approx 43.67 \text{ s}
$$

## Final Result
* **Heading Angle:** $23.58^\circ$ upstream (West of North).
* **Crossing Time:** $43.67 \text{ s}$.

## Interpretation
To compensate for the river's current, the boat must aim upstream. This reduces its effective speed across the river compared to its speed in still water.
