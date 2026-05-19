# Task 06 – Instrument Precision

## Problem Statement
A digital thermometer reads $25.4^\circ\text{C}$. Assuming the uncertainty is half the value of the last digit, what is the absolute uncertainty of this measurement?

## Theory
For digital instruments, readings change in discrete increments rather than continuous scales. The finest graduation or the smallest increment that a digital display can record is known as the instrument's resolution (or least count).

When explicit manufacturer calibration data is unavailable, a standard conservative convention in laboratory physics states that the absolute uncertainty $\Delta x$ is equal to half the value of the smallest readable digit (the last decimal place):

$$
\Delta x = \frac{1}{2} \cdot (\text{Resolution})
$$

## Step-by-Step Solution
Identify the last digit of the displayed value:

$$
T = 25.4^\circ\text{C}
$$

The last visible digit resides in the tenths place. Therefore, the resolution (the smallest structural step the display can register) is:

$$
\text{Resolution} = 0.1^\circ\text{C}
$$

Apply the criteria provided in the problem statement to calculate the absolute uncertainty $\Delta T$:

$$
\begin{align}
\Delta T &= \frac{1}{2} \cdot 0.1^\circ\text{C} \\
         &= 0.05^\circ\text{C}
\end{align}
$$

Combine the central value with its calculated boundary error to express the complete physical measurement:

## Final Result

$$
\Delta T = 0.05^\circ\text{C}
$$

The complete measurement is recorded as:

$$
T = (25.40 \pm 0.05)^\circ\text{C}
$$

## Interpretation
An absolute uncertainty of $0.05^\circ\text{C}$ establishes that the true thermodynamic temperature falls safely within the interval of $[25.35^\circ\text{C}, 24.45^\circ\text{C}]$. Because digital displays truncate or round values automatically, this interval reflects the inherent precision limits of the analog-to-digital converter inside the thermometer.