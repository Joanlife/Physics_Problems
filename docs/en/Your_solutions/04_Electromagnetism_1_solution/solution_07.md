# Task 07 – Cyclotron Motion

## Problem Statement

An electron is accelerated from rest through a potential difference of $5000$ V. It then enters a region of uniform magnetic field $B = 0.1$ T, perpendicular to its velocity. What is the radius of the circular path it will follow?

## Theory

This problem combines two major concepts in electromagnetism: **Energy Conservation** and **Magnetic Force**.

1. **Acceleration:** When a charge $q$ is accelerated through a potential $V$, it gains kinetic energy $K$:
   $$
   qV = \frac{1}{2} mv^2
   $$

2. **Magnetic Motion:** When a charge enters a magnetic field perpendicular to its velocity, the Lorentz force acts as a centripetal force:
   $$
   qvB = \frac{mv^2}{R}
   $$
   Rearranging for the radius $R$:
   $$
   R = \frac{mv}{qB}
   $$

**Constants:**
- $m_e \approx 9.11 \times 10^{-31} \text{ kg}$
- $q_e \approx 1.6 \times 10^{-19} \text{ C}$

## Step-by-Step Solution

### 1. Calculate the Velocity ($v$)
First, find the speed of the electron after acceleration:
$$
v = \sqrt{\frac{2qV}{m}} = \sqrt{\frac{2(1.6 \times 10^{-19})(5000)}{9.11 \times 10^{-31}}}
$$
$$
v \approx \sqrt{1.756 \times 10^{15}} \approx 4.19 \times 10^7 \text{ m/s}
$$

### 2. Calculate the Radius ($R$)
Now, substitute this velocity into the radius formula:
$$
R = \frac{(9.11 \times 10^{-31})(4.19 \times 10^7)}{(1.6 \times 10^{-19})(0.1)}
$$
$$
R \approx \frac{3.817 \times 10^{-23}}{1.6 \times 10^{-20}}
$$
$$
R \approx 0.00238 \text{ m}
$$

## Final Result

The radius of the circular path is:
$$
R \approx 2.38 \text{ mm}
$$

## Interpretation

The electron moves in a very tight circle. This is because electrons are extremely light (low mass), making them very "responsive" to magnetic fields. In a presentation, you could explain that this principle is used in devices like mass spectrometers and particle accelerators (cyclotrons) to control the path of charged particles.