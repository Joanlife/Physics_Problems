# Task 08 – Mass-Spring Measurements (Theory & Data Processing)

## Problem Statement
Using data from a simulator of a mass suspended on a spring, perform 10 time measurements for 10 complete oscillations. Calculate the mean period, standard deviation, the spring constant, and its measurement uncertainty.

## Theory
The period $T$ of a simple mass-spring system undergoing simple harmonic motion is:

$$
T = 2\pi \sqrt{\frac{m}{k}}
$$

Rearranging this formula to solve for the spring constant $k$ yields:

$$
k = \frac{4\pi^2 m}{T^2}
$$

When timing $10$ oscillations, the period is $T = t_{10} / 10$. The uncertainty in the period $\Delta T$ is derived from the standard deviation of the repeated measurements. The relative uncertainty for $k$ is given by propagating the error from $T$:

$$
\frac{\Delta k}{k} = 2 \frac{\Delta T}{T}
$$

## Step-by-Step Solution
*(Note: As data must be gathered from an external HTML simulator, the steps below outline the strict mathematical procedure required once data is obtained.)*

1.  **Find Mean Period:** Record times $t_1, t_2, \dots, t_{10}$ for 10 oscillations. Divide each by 10 to get individual periods $T_1, T_2, \dots, T_{10}$. Compute the mean $\bar{T}$.
2.  **Determine Standard Deviation:** Use the sample standard deviation formula on the $T_i$ values to find $\sigma_T$, which serves as the absolute uncertainty $\Delta T$.
3.  **Calculate Spring Constant:** Substitute the given mass $m$ and the mean period $\bar{T}$ into the rearranged formula for $k$.
4.  **Calculate Uncertainty in k:** Multiply the calculated $k$ by $2(\Delta T / \bar{T})$ to isolate $\Delta k$.

## Final Result
The final calculated value will take the form:

$$
k = (k_{calculated} \pm \Delta k) \text{ N/m}
$$

## Interpretation
Taking the time for 10 oscillations reduces human reaction time error by a factor of 10. Because $k \propto 1/T^2$, any percentage error in the measurement of the period will be doubled when determining the final uncertainty of the spring constant.