# Task 09 – Pendulum Measurements

## Problem Statement
Using an HTML simulator or a physical setup, perform 10 measurements of the time taken for 10 complete oscillations of a simple pendulum. Assuming the string length is exact, calculate the mean period, standard deviation, the acceleration due to gravity, and its associated measurement uncertainty.

## Theory
The period $T$ of a simple pendulum for small angle oscillations is governed by the length of the string $L$ and the acceleration due to gravity $g$:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Rearranging the formula to isolate the acceleration due to gravity yields:

$$
g = \frac{4\pi^2 L}{T^2}
$$

To minimize timing errors, the time for 10 oscillations ($t_{10}$) is recorded, and the period is computed as $T = t_{10} / 10$. The absolute uncertainty in the period, $\Delta T$, is derived from the sample standard deviation of the repeated measurements.

Assuming the length $L$ is an exact value with negligible error, the relative uncertainty in $g$ is determined entirely by the uncertainty in the period. Applying the power rule for error propagation provides:

$$
\frac{\Delta g}{g} = 2 \frac{\Delta T}{T}
$$

## Step-by-Step Solution
*(Note: As data collection requires an experiment or simulation, the following protocol defines the exact mathematical procedure to process the data once obtained.)*

1. **Calculate Individual Periods:** Record the 10 elapsed times $t_1, t_2, \dots, t_{10}$ for 10 full oscillations. Divide each by 10 to obtain the dataset of individual periods $T_1, T_2, \dots, T_{10}$.
2. **Calculate Mean Period:**

$$
\bar{T} = \frac{1}{10} \sum_{i=1}^{10} T_i
$$

3. **Calculate Standard Deviation:** Compute the sample standard deviation to establish the absolute uncertainty $\Delta T$:

$$
\Delta T = \sqrt{\frac{1}{10 - 1} \sum_{i=1}^{10} (T_i - \bar{T})^2}
$$

4. **Calculate Central Value of g:** Substitute the mean period $\bar{T}$ and the known length $L$ into the gravity equation to find $g$.
5. **Calculate Absolute Uncertainty in g:** Substitute the computed values into the error propagation formula and solve for $\Delta g$:

$$
\Delta g = g \left( 2 \frac{\Delta T}{\bar{T}} \right)
$$

## Final Result
The final measurement for the acceleration due to gravity will be reported in the standard format:

$$
g = (g_{calculated} \pm \Delta g) \text{ m/s}^2
$$

## Interpretation
Measuring 10 consecutive oscillations significantly reduces the fractional error introduced by human reaction time at the start and stop of the stopwatch. Furthermore, the inverse-square relationship ($g \propto 1/T^2$) dictates that the relative uncertainty in the calculated value of $g$ is twice as large as the relative uncertainty in the period measurement.