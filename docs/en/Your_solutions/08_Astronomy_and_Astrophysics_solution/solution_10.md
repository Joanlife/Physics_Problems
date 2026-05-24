# Task 10 – Measuring the Height of the Atmosphere

## Problem Statement

A medieval astronomer in Al-Andalus, Al-Zarqali (Arzachel) (1029–1087 AD), attempted to estimate the height of the Earth’s atmosphere using a geometric method based on sunset timing. He measured the interval between sunset and the moment when faint stars first became visible, assuming that this corresponds to the Sun reaching a true geometric depression angle $\phi$ below the horizon. A chronicle reports that on a clear evening the time between sunset and the first appearance of faint stars was $t = 40$ minutes.

Assume:
* Earth radius $R_E = 6370\,\text{km}$
* Earth’s rotation rate: full rotation in 24 hours (i.e., $360^\circ$ in 24 hours)
* A simple “sharp-edge atmosphere” model in which a Sun ray reaches the observer by just grazing the top of the atmosphere, giving

$$
\cos\phi = \frac{R_E}{R_E+h}
$$

Find:
1. The solar depression angle $\phi$ (in degrees) implied by the measured time $t$.
2. The atmospheric height $h$ in km.

## Theory

The Earth rotates at a constant angular velocity. Because a full rotation takes 24 hours, the angular speed $\omega$ in degrees per minute is determined by dividing $360^\circ$ by the total minutes in a day. 

$$
\omega = \frac{360^\circ}{24 \times 60\,\text{min}}
$$

The solar depression angle $\phi$ is simply the angle the Earth rotates through during the observed time interval $t$.

$$
\phi = \omega t
$$

The sharp-edge geometric model forms a right triangle. The distance from Earth's center to the observer is the adjacent side ($R_E$), and the distance from Earth's center to the grazing point at the top of the atmosphere is the hypotenuse ($R_E + h$).

Rearranging the given cosine relation to solve for $h$ yields

$$
\begin{align}
R_E + h &= \frac{R_E}{\cos\phi} \\
      h &= R_E \left( \frac{1}{\cos\phi} - 1 \right)
\end{align}
$$

## Step-by-Step Solution

First, calculate the angular rotation rate of the Earth.

$$
\omega = \frac{360^\circ}{1440\,\text{min}} = 0.25^\circ/\text{min}
$$

Next, determine the solar depression angle for the 40-minute twilight duration.

$$
\phi = 0.25^\circ/\text{min} \times 40\,\text{min} = 10^\circ
$$

Now, substitute this angle and the Earth's radius into the rearranged height formula. 

$$
h = 6370\,\text{km} \times \left( \frac{1}{\cos(10^\circ)} - 1 \right)
$$

Evaluate the trigonometric term.

$$
\cos(10^\circ) \approx 0.98480775
$$

Calculate the ratio of the hypotenuse to the adjacent side.

$$
\frac{1}{0.98480775} \approx 1.0154266
$$

Subtract the baseline Earth radius fraction.

$$
1.0154266 - 1 = 0.0154266
$$

Multiply by the Earth's radius to find the final height.

$$
h = 6370 \times 0.0154266 \approx 98.268\,\text{km}
$$

## Final Result

1. The solar depression angle $\phi$ is exactly $10^\circ$.
2. The atmospheric height $h$ is approximately $98.3\,\text{km}$.

## Interpretation

This ancient calculation yields an answer remarkably close to the modern Karman line, which places the edge of space at $100\,\text{km}$. While the "sharp-edge" geometric model ignores atmospheric refraction (which bends light around the Earth) and the gradual thinning of the atmosphere, it demonstrates how precise timing and basic geometry can produce excellent scientific estimates.