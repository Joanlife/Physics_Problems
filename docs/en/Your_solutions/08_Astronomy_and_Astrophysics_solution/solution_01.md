# Task 01 – Rotational Velocity

## Problem Statement

Calculate the linear speed (in km/s) of a point on the Earth's equator due to its rotation. Earth's radius is approximately $6378$ km.

## Theory

The linear speed $v$ of a point on a rotating spherical body depends on its radial distance from the rotational axis and its angular velocity. At the equator, the distance from the rotational axis equals the full radius of the Earth $R_E$.

The angular velocity $\omega$ of a rotating body with a rotational period $T$ is given by

$$
\omega = \frac{2\pi}{T}
$$

The relationship between linear velocity $v$ and angular velocity $\omega$ at a distance $R_E$ from the axis of rotation is defined by

$$
v = \omega R_E
$$

Substituting the expression for angular velocity into the linear velocity equation yields

$$
v = \frac{2\pi R_E}{T}
$$

## Step-by-Step Solution

To calculate the linear speed at the equator, the physical parameters must first be expressed in consistent SI units or standard units appropriate for the target output ($\text{km/s}$).

The given radius of the Earth at the equator is

$$
R_E = 6378\,\text{km}
$$

The rotational period of the Earth relative to the Sun (one solar day) is exactly 24 hours. Converting this period into seconds yields

$$
\begin{align}
T &= 24\,\text{hours} \times 60\,\frac{\text{minutes}}{\text{hour}} \times 60\,\frac{\text{seconds}}{\text{minute}} \\
  &= 86400\,\text{s}
\end{align}
$$

Substituting these values into the linear speed formula gives

$$
v = \frac{2 \pi \times 6378\,\text{km}}{86400\,\text{s}}
$$

Calculating the numerator presents the total equatorial circumference

$$
2 \pi \times 6378\,\text{km} \approx 40074.16\,\text{km}
$$

Dividing by the total seconds in a solar day yields

$$
v \approx \frac{40074.16\,\text{km}}{86400\,\text{s}} \approx 0.46382\,\text{km/s}
$$





## Final Result

The linear speed of a point on the Earth's equator due to its axial rotation is approximately $0.464\,\text{km/s}$ 

## Interpretation

Although a person standing on the equator feels stationary, they are moving through space at nearly half a kilometer per second due to planetary rotation. This high linear velocity has significant practical applications in aerospace engineering. Launching rockets close to the equator in the prograde direction (eastward) allows vehicles to inherit this initial speed, reducing the total chemical delta-v required to achieve stable low Earth orbit.