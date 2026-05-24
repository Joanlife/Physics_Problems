# Task 06 – Solar Gravity

## Problem Statement

Calculate the acceleration due to gravity on the surface of the Sun. By what factor would an observer's weight increase if they could stand on its surface? The Sun's mass is $M_S \approx 2 \times 10^{30}$ kg and its radius is $R_S \approx 6.96 \times 10^8$ m. Assume Earth's surface gravity is $g_E \approx 9.81$ m/s².

## Theory

The surface gravity of a spherical celestial body is calculated directly from Newton's field equations. The mass is assumed to act as a point source concentrated at the center of the sphere for all positions at or beyond the surface radius.

$$
g = \frac{G M}{R^2}
$$

The weight of an object is the net force exerted on it by gravity, defined by $W = mg$. Because mass $m$ remains invariant across environments, the scale factor change in weight matches the exact ratio of the local gravitational accelerations

$$
\text{Weight Factor} = \frac{g_S}{g_E}
$$

## Step-by-Step Solution

Identify the operational solar criteria provided

$$
G = 6.6743 \times 10^{-11}\,\text{m}^3\,\text{kg}^{-1}\,\text{s}^{-2}
$$

$$
M_S = 2 \times 10^{30}\,\text{kg}
$$

$$
R_S = 6.96 \times 10^8\,\text{m}
$$

Square the solar radius value

$$
R_S^2 = (6.96 \times 10^8)^2 = 4.84416 \times 10^{17}\,\text{m}^2
$$

Compute the numerator parameter

$$
G M_S = 6.6743 \times 10^{-11} \times 2 \times 10^{30} = 1.33486 \times 10^{20}\,\text{m}^3\,\text{s}^{-2}
$$

Divide to find the solar gravitational field strength

$$
g_S = \frac{1.33486 \times 10^{20}}{4.84416 \times 10^{17}} \approx 275.561\,\text{m/s}^2
$$

Calculate the magnification index relative to Earth's baseline environment

$$
\text{Factor} = \frac{275.561\,\text{m/s}^2}{9.81\,\text{m/s}^2} \approx 28.09
$$

## Final Result

The acceleration due to gravity on the surface of the Sun is approximately $275.6\,\text{m/s}^2$. Consequently, an observer's weight would increase by a factor of $28.1$ times.

## Interpretation

Even though the Sun's radius is huge ($109$ times greater than Earth's), which reduces surface gravity due to the inverse-square law, its mass is incredibly large ($333000$ times greater than Earth's). The massive quantity of matter completely wins out over the large radius, producing a surface gravity 28 times stronger than Earth's. A human weighing $80\,\text{kg}$ on Earth would experience a gravitational force equivalent to over $2200\,\text{kg}$ on the Sun, structural loads far exceeding biological survival limits.