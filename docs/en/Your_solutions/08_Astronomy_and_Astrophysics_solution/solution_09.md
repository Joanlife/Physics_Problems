# Task 09 – Size and Distance of the Sun

## Problem Statement

Aristarchus of Samos (310–230 BC) used geometric observations of lunar phases to estimate the relative distances and sizes of the Sun and the Moon. At the exact half-Moon phase (dichotomy), the Earth–Moon–Sun system forms a right triangle with the right angle located at the Moon. 

The observed angular separation between the Sun and the Moon from Earth is $\theta = 89.85^\circ$. The apparent angular diameter of both bodies is $\alpha = 0.53^\circ$. The average Earth–Moon distance is $d_{EM} = 3.84 \times 10^5\,\text{km}$.

Calculate:
1. The Earth–Sun distance $d_{ES}$ in km.
2. The true diameter of the Sun $D_S$ in km using the small-angle approximation.
3. The ratio of true diameters $\frac{D_M}{D_S}$.
4. The value of $d_{ES}$ if the historical measurement $\theta = 89.75^\circ$ is used instead. Comment on the stability and sensitivity of this measurement approach.

## Theory

Because the Earth–Moon–Sun system forms a right triangle during the half-moon phase, simple right-triangle trigonometry applies. The Earth-Moon distance acts as the adjacent side to angle $\theta$, while the Earth-Sun distance forms the hypotenuse.



$$
\cos\theta = \frac{d_{EM}}{d_{ES}} \implies d_{ES} = \frac{d_{EM}}{\cos\theta}
$$

The small-angle approximation states that for a small angle $\alpha$ measured in radians, the linear size $D$ of an object at a distance $d$ can be approximated by

$$
\alpha \approx \frac{D}{d} \implies D = \alpha_{\text{rad}} \times d
$$

To convert an angle from degrees to radians, the conversion factor is

$$
\alpha_{\text{rad}} = \alpha^\circ \times \frac{\pi}{180^\circ}
$$

## Step-by-Step Solution

### 1. Calculation of Earth–Sun Distance ($d_{ES}$)

For $\theta = 89.85^\circ$:

$$
\cos(89.85^\circ) = \sin(90^\circ - 89.85^\circ) = \sin(0.15^\circ) \approx 0.00261799
$$

Substitute this value into the geometric equation

$$
d_{ES} = \frac{3.84 \times 10^5\,\text{km}}{0.00261799} \approx 1.46677 \times 10^8\,\text{km}
$$

### 2. Calculation of True Sun Diameter ($D_S$)

Convert the apparent angular diameter $\alpha = 0.53^\circ$ into radians

$$
\alpha_{\text{rad}} = 0.53^\circ \times \frac{\pi}{180^\circ} \approx 0.00925025\,\text{rad}
$$

Apply the small-angle equation using the calculated distance $d_{ES}$

$$
D_S = 0.00925025 \times 1.46677 \times 10^8\,\text{km} \approx 1.35679 \times 10^6\,\text{km}
$$

### 3. Calculation of Diameter Ratio ($\frac{D_M}{D_S}$)

Because both bodies exhibit identical apparent angular diameters ($\alpha = 0.53^\circ$), their true sizes are directly proportional to their distances

$$
D_M = \alpha_{\text{rad}} d_{EM},\quad D_S = \alpha_{\text{rad}} d_{ES}
$$

$$
\frac{D_M}{D_S} = \frac{\alpha_{\text{rad}} d_{EM}}{\alpha_{\text{rad}} d_{ES}} = \frac{d_{EM}}{d_{ES}} = \cos\theta
$$

Substituting the cosine value from part 1 gives

$$
\frac{D_M}{D_S} = \cos(89.85^\circ) \approx 0.002618 = \frac{1}{382}
$$

### 4. Sensitivity Analysis ($\theta = 89.75^\circ$)

Recalculate the distance using Aristarchus' alternative historical angle constraint

$$
\cos(89.75^\circ) = \sin(0.25^\circ) \approx 0.00436331
$$

$$
d_{ES}' = \frac{3.84 \times 10^5\,\text{km}}{0.00436331} \approx 8.80066 \times 10^7\,\text{km}
$$

Calculate the total absolute difference caused by this tiny angle variation

$$
\Delta d_{ES} = 1.46677 \times 10^8\,\text{km} - 8.80066 \times 10^7\,\text{km} \approx 5.867 \times 10^7\,\text{km}
$$

## Final Result

1. The Earth–Sun distance is $146.7\,\text{million kilometers}$.
2. The physical diameter of the Sun is $1.357 \times 10^6\,\text{km}$.
3. The ratio of the Moon's diameter to the Sun's diameter is $0.00262$ ($\approx 1/382$).
4. Changing the input observation angle by a tiny $0.10^\circ$ (to $89.75^\circ$) shifts the calculated distance down to $88.0\,\text{million kilometers}$, a reduction of $40\%$.

## Interpretation

This calculation shows that Aristarchus' method is mathematically brilliant but highly sensitive to small measurement errors. Because the true angle is very close to a right angle ($90^\circ$), the cosine function drops off extremely fast. A tiny error in measuring the angle by a fraction of a degree leads to a massive change in the calculated distance. Without high-precision telescopes, Aristarchus could not measure the angle accurately enough to get the true distance, but his geometry successfully proved that the Sun is significantly larger than the Earth and located extremely far away.