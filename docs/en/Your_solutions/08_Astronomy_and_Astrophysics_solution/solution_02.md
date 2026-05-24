# Task 02 – Orbital Mechanics

## Problem Statement

Calculate the orbital speed of the International Space Station (ISS), which orbits at an altitude of approximately 400 km above the Earth's surface. The Earth's mass is $M_E \approx 5.97 \times 10^{24}$ kg and its radius is $R_E \approx 6378$ km. Compare this speed to the Earth's orbital speed around the Sun, assuming an Earth–Sun distance of $d_{ES} \approx 150 \times 10^6$ km and an orbital period of $T_E \approx 365.25$ days. Determine which system exhibits a faster orbital velocity.

## Theory

For any object in a stable circular orbit around a dominant central mass, the gravitational force provides the necessary centripetal force. The mathematical equilibrium is expressed as

$$
F_g = F_c
$$

Substituting Newton's law of universal gravitation and the classical mechanics definition of centripetal force gives

$$
\frac{G M m}{r^2} = \frac{m v^2}{r}
$$

where $G$ is the gravitational constant, $M$ is the mass of the central body, $m$ is the mass of the orbiting satellite, $r$ is the orbital radius measured from the center of the central mass, and $v$ is the tangential orbital velocity. Solving for $v$ yields the orbital speed formula

$$
v = \sqrt{\frac{G M}{r}}
$$

For a satellite at an altitude $h$ above a planet's surface, the total orbital radius is

$$
r = R + h
$$

For a large planetary body orbiting a star in a circular path, the average orbital velocity can also be determined from the geometric path length over its orbital period

$$
v = \frac{2\pi d}{T}
$$

## Step-by-Step Solution

### 1. Calculation of ISS Orbital Velocity

The constant values and system configurations are defined as

$$
G = 6.6743 \times 10^{-11}\,\text{m}^3\,\text{kg}^{-1}\,\text{s}^{-2}
$$

$$
M_E = 5.97 \times 10^{24}\,\text{kg}
$$

$$
R_E = 6378\,\text{km} = 6.378 \times 10^6\,\text{m}
$$

$$
h = 400\,\text{km} = 4.00 \times 10^5\,\text{m}
$$

Calculate the total orbital radius of the space station

$$
r_{ISS} = 6.378 \times 10^6\,\text{m} + 4.00 \times 10^5\,\text{m} = 6.778 \times 10^6\,\text{m}
$$

Substitute these values into the orbital speed formula

$$
v_{ISS} = \sqrt{\frac{6.6743 \times 10^{-11} \times 5.97 \times 10^{24}}{6.778 \times 10^6}}
$$

Compute the standard gravitational parameter in the numerator

$$
G M_E = 3.98456 \times 10^{14}\,\text{m}^3\,\text{s}^{-2}
$$

Divide by the orbital radius

$$
\frac{3.98456 \times 10^{14}}{6.778 \times 10^6} \approx 5.87866 \times 10^7\,\text{m}^2\,\text{s}^{-2}
$$

Extract the square root to determine velocity

$$
v_{ISS} = \sqrt{5.87866 \times 10^7} \approx 7667.24\,\text{m/s} \approx 7.67\,\text{km/s}
$$

### 2. Calculation of Earth's Orbital Velocity Around the Sun

The parameters of Earth's orbit are given as

$$
d_{ES} = 150 \times 10^6\,\text{km} = 1.50 \times 10^{11}\,\text{m}
$$

$$
T_E = 365.25\,\text{days}
$$

Convert the orbital period into standard SI seconds

$$
\begin{align}
T_E &= 365.25\,\text{days} \times 24\,\frac{\text{hours}}{\text{day}} \times 3600\,\frac{\text{seconds}}{\text{hour}} \\
    &= 31557600\,\text{s}
\end{align}
$$

Calculate the velocity using the circular path configuration

$$
v_E = \frac{2 \pi \times 1.50 \times 10^{11}\,\text{m}}{31557600\,\text{s}}
$$

$$
v_E \approx \frac{9.42478 \times 10^{11}}{31557600} \approx 29865.32\,\text{m/s} \approx 29.87\,\text{km/s}
$$

### 3. Comparison

Comparing the calculated velocities shows

$$
v_E \approx 29.87\,\text{km/s} > v_{ISS} \approx 7.67\,\text{km/s}
$$

## Final Result

The orbital speed of the International Space Station is approximately $7.67\,\text{km/s}$. The orbital speed of the Earth around the Sun is approximately $29.87\,\text{km/s}$. The Earth traveling around the Sun is faster than the ISS traveling around the Earth by a factor of roughly $3.9$.

## Interpretation

Orbital velocity is inversely proportional to the square root of the orbital radius, but directly proportional to the square root of the central mass being orbited. Even though the Earth–Sun distance is massive compared to the radius of low Earth orbit, the immense gravitational mass of the Sun ($M_S \approx 333000 M_E$) dominates the dynamical equation, requiring a much higher velocity for the Earth to maintain its orbit.