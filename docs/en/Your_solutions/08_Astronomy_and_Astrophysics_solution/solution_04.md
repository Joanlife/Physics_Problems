# Task 04 – Geostationary Orbit

## Problem Statement

Satellites in geostationary orbit (GEO) must remain stationary above a fixed point on Earth's equator. What must their orbital period be? Calculate the precise altitude of a geostationary orbit above the Earth's surface.

## Theory

For a satellite to remain fixed over a specific geographical coordinate on the equator, its orbital period $T$ must precisely match the rotational period of the Earth relative to the inertial frame of the stars. This period is one sidereal day, which is shorter than a solar day due to the Earth's simultaneous orbital movement around the Sun.

$$
T = 23\,\text{hours}\,56\,\text{minutes}\,4.1\,\text{seconds} = 86164.1\,\text{s}
$$

Equating gravitational force and centripetal force leads to Kepler's Third Law for circular paths

$$
\frac{G M_E}{r^2} = \omega^2 r
$$

Substituting the angular frequency $\omega = \frac{2\pi}{T}$ into the equation gives

$$
\frac{G M_E}{r^2} = \left(\frac{2\pi}{T}\right)^2 r = \frac{4\pi^2 r}{T^2}
$$

Isolating the orbital radius $r$ results in the expression

$$
r^3 = \frac{G M_E T^2}{4\pi^2} \implies r = \sqrt[3]{\frac{G M_E T^2}{4\pi^2}}
$$

The altitude $h$ above the Earth's surface is then computed by subtracting the planetary equatorial radius

$$
h = r - R_E
$$

## Step-by-Step Solution

Define the physical constants of the Earth system

$$
G M_E = 3.98456 \times 10^{14}\,\text{m}^3\,\text{s}^{-2}
$$

$$
R_E = 6378\,\text{km} = 6.378 \times 10^6\,\text{m}
$$

$$
T = 86164.1\,\text{s}
$$

Square the sidereal period

$$
T^2 = (86164.1)^2 \approx 7.42425 \times 10^9\,\text{s}^2
$$

Multiply by the standard gravitational parameter

$$
G M_E T^2 = (3.98456 \times 10^{14}) \times (7.42425 \times 10^9) \approx 2.95825 \times 10^{24}\,\text{m}^3
$$

Divide by the angular constant term

$$
\frac{G M_E T^2}{4\pi^2} = \frac{2.95825 \times 10^{24}}{39.47842} \approx 7.49334 \times 10^{22}\,\text{m}^3
$$

Extract the cube root to find the total orbital radius from the center of mass

$$
r = \sqrt[3]{7.49334 \times 10^{22}} \approx 4.21641 \times 10^7\,\text{m} \approx 42164.1\,\text{km}
$$

Calculate the altitude by subtracting the surface radius

$$
h = 42164.1\,\text{km} - 6378\,\text{km} = 35786.1\,\text{km}