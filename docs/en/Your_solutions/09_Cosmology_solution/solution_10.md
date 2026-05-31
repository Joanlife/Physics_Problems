# Task 10 – Doppler Effect

## Problem Statement

A galaxy is receding from Earth at a speed of $5 \times 10^6 \text{ m/s}$. It emits light with a wavelength of 486 nm. What wavelength will be observed on Earth? 
Calculate using the non-relativistic formula: $\lambda_{observed} = \lambda_{emitted} \left(1 + \frac{v}{c}\right)$.
Calculate using the relativistic formula: $\lambda_{observed} = \lambda_{emitted} \sqrt{\frac{1 + v/c}{1 - v/c}}$.
Compare the results.

## Theory

The Doppler effect for electromagnetic waves causes a shift in observed wavelength when the source is moving relative to the observer. 

For velocities significantly lower than the speed of light, the non-relativistic linear approximation is sufficient. For higher velocities, the exact relativistic formulation derived from Lorentz transformations is required to account for time dilation.

$$
\beta = \frac{v}{c}
$$

## Step-by-Step Solution

1. Define the given variables:

$$
v = 5 \times 10^6 \text{ m/s}
$$

$$
c \approx 3 \times 10^8 \text{ m/s}
$$

$$
\lambda_{emitted} = 486 \text{ nm}
$$

2. Calculate the beta factor ($\beta$):

$$
\beta = \frac{5 \times 10^6}{3 \times 10^8} \approx 0.01667
$$

3. Calculate the observed wavelength using the non-relativistic formula:

$$
\begin{align}
\lambda_{non-rel} &= 486 \left(1 + 0.01667\right) \\
&= 486 \times 1.01667 \\
&\approx 494.10 \text{ nm}
\end{align}
$$

4. Calculate the observed wavelength using the relativistic formula:

$$
\begin{align}
\lambda_{rel} &= 486 \sqrt{\frac{1 + 0.01667}{1 - 0.01667}} \\
&= 486 \sqrt{\frac{1.01667}{0.98333}} \\
&= 486 \sqrt{1.0339} \\
&= 486 \times 1.0168 \\
&\approx 494.17 \text{ nm}
\end{align}
$$

## Final Result

* Non-relativistic observed wavelength: $\approx 494.10 \text{ nm}$
* Relativistic observed wavelength: $\approx 494.17 \text{ nm}$

## Interpretation

The results are extremely close, differing by only $0.07 \text{ nm}$. This indicates that at a recession velocity of $1.67\%$ the speed of light, the non-relativistic approximation remains highly accurate, though the relativistic calculation is technically the exact solution. Both calculations correctly demonstrate a "redshift" toward a longer wavelength.