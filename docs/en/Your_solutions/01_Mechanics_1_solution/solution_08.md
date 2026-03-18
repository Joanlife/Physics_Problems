# Task 08 – Circular Motion (Equatorial Acceleration)

## Problem Statement
Calculate the centripetal acceleration $a_c$ of a person standing on the Earth's equator. The Earth's radius is approximately $R = 6378 \text{ km}$.

## Theory
An object moving in a circular path of radius $R$ at a constant speed $v$ undergoes centripetal acceleration. This acceleration is always directed toward the center of the circle.

The relationship between linear velocity $v$ and angular velocity $\omega$ is given by:

$$
v = \omega R
$$

Substituting this into the standard formula for centripetal acceleration $a_c = \frac{v^2}{R}$:

$$
a_c = \frac{(\omega R)^2}{R} = \frac{\omega^2 R^2}{R} = \omega^2 R
$$



## Step-by-Step Solution

### 1. Determining Angular Velocity ($\omega$)
The Earth completes one full rotation ($2\pi$ radians) in approximately 24 hours.

$$
T = 24 \text{ h} \times 3600 \text{ s/h} = 86400 \text{ s}
$$

The angular velocity is:

$$
\omega = \frac{2\pi}{T} = \frac{2\pi}{86400} \approx 7.272 \times 10^{-5} \text{ rad/s}
$$

### 2. Converting Units
The radius of the Earth must be in meters for the SI unit of acceleration ($\text{m/s}^2$):

$$
R = 6378 \text{ km} = 6.378 \times 10^6 \text{ m}
$$

### 3. Calculating Centripetal Acceleration
Using the derived formula $a_c = \omega^2 R$:

$$
a_c = (7.272 \times 10^{-5} \text{ rad/s})^2 \cdot (6.378 \times 10^6 \text{ m})
$$

$$
a_c \approx (5.288 \times 10^{-9}) \cdot (6.378 \times 10^6)
$$

$$
a_c \approx 0.0337 \text{ m/s}^2
$$

## Final Result
The centripetal acceleration at the equator is approximately **$0.0337 \text{ m/s}^2$**.

## Interpretation
While the Earth's rotation speed at the equator is quite high (approx. $460 \text{ m/s}$), the radius is so large that the resulting centripetal acceleration is minimal. It represents only about $0.34\%$ of the acceleration due to gravity ($g \approx 9.81 \text{ m/s}^2$), which is why we do not feel the rotational motion in our daily lives.