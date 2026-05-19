# Task 04 – Relative Uncertainty

## Problem Statement
A car's speedometer has a $5\%$ uncertainty. If it reads $60 \text{ km/h}$, what is the range of the car's actual speed?

## Theory
Percentage uncertainty represents the relative error expressed as a percentage. The absolute uncertainty $\Delta v$ of a measured quantity $v$ is calculated by multiplying the measured value by the fractional uncertainty:

$$
\Delta v = v \cdot \left( \frac{\text{Percentage Uncertainty}}{100} \right)
$$

The possible range of the actual value is then defined by the interval spanning from the measured value minus the absolute uncertainty, to the measured value plus the absolute uncertainty:

$$
[v - \Delta v, v + \Delta v]
$$

## Step-by-Step Solution
Identify the measured speed $v$ and its associated relative error:

$$
v = 60 \text{ km/h}
$$

Convert the $5\%$ uncertainty to a decimal and calculate the absolute uncertainty $\Delta v$:

$$
\begin{align}
\Delta v &= 60 \cdot 0.05 \\
         &= 3 \text{ km/h}
\end{align}
$$

Calculate the lower bound of the speed range:

$$
\begin{align}
v_{min} &= v - \Delta v \\
        &= 60 - 3 \\
        &= 57 \text{ km/h}
\end{align}
$$

Calculate the upper bound of the speed range:

$$
\begin{align}
v_{max} &= v + \Delta v \\
        &= 60 + 3 \\
        &= 63 \text{ km/h}
\end{align}
$$

## Final Result

$$
v = (60 \pm 3) \text{ km/h}
$$

The range of the car's actual speed is $[57, 63] \text{ km/h}$.

## Interpretation
A relative uncertainty of $5\%$ means that the actual speed can deviate by up to $3 \text{ km/h}$ in either direction from the reading. Therefore, a dashboard reading of $60 \text{ km/h}$ bounds the physical speed of the vehicle strictly between $57 \text{ km/h}$ and $63 \text{ km/h}$.