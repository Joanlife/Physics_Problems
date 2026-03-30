# Task 01 – Gravitational Dependence of a Pendulum

## Problem Statement

A simple pendulum has a period of $4\text{ s}$ on Earth. 

1. What would its period be on the Moon, where the gravitational acceleration is about $1/6$th of Earth's?
2. What is the required length of a simple pendulum to have a period of exactly $1\text{ s}$ on Earth?

## Theory

The period $T$ of a simple pendulum undergoing small-angle oscillations is given by the formula:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Where:
* $L$ is the length of the pendulum string.
* $g$ is the acceleration due to gravity.

The relationship shows that the period is directly proportional to the square root of the length and inversely proportional to the square root of the gravitational acceleration.

## Step-by-Step Solution

### Part 1: Period on the Moon

Let $T_E = 4\text{ s}$ and $g_E$ be the gravity on Earth. On the Moon, the gravity is $g_M = \frac{1}{6}g_E$. We write the ratio of the periods:

$$
\frac{T_M}{T_E} = \frac{2\pi \sqrt{\frac{L}{g_M}}}{2\pi \sqrt{\frac{L}{g_E}}}
$$

$$
\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_M}}
$$

Substituting $g_M = \frac{1}{6}g_E$:

$$
\frac{T_M}{T_E} = \sqrt{\frac{g_E}{\frac{1}{6}g_E}} = \sqrt{6}
$$

$$
T_M = T_E \cdot \sqrt{6} = 4\sqrt{6} \approx 9.80\text{ s}
$$

### Part 2: Required Length on Earth

To find the length $L$ for a specific period $T = 1\text{ s}$, we rearrange the period formula:

$$
T^2 = 4\pi^2 \frac{L}{g}
$$

$$
L = \frac{T^2 g}{4\pi^2}
$$

Using $g \approx 9.81\text{ m/s}^2$ and $T = 1\text{ s}$:

$$
L = \frac{1^2 \cdot 9.81}{4\pi^2} \approx \frac{9.81}{39.478} \approx 0.248\text{ m}
$$

## Final Result

1. The period on the Moon is $T_M = 4\sqrt{6} \approx 9.80\text{ s}$.
2. The required length on Earth is $L \approx 0.248\text{ m}$ (or $24.8\text{ cm}$).

## Interpretation

The period increases on the Moon because the restoring force (gravity) is weaker, causing the pendulum to swing more slowly. To achieve a shorter period of $1\text{ s}$ on Earth, the pendulum must be significantly shorter than the one that produces a $4\text{ s}$ period.