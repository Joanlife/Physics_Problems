# Task 03 – Propagation of Error III

## Problem Statement
The resistance $R$ is calculated using Ohm's Law, $R = V/I$. If the voltage is measured as $V = (10.0 \pm 0.2)\text{ V}$ and the current as $I = (2.00 \pm 0.05)\text{ A}$, what is the calculated resistance and its uncertainty?

## Theory
According to Ohm's Law, electrical resistance is the ratio of voltage to current:

$$
R = \frac{V}{I}
$$

For the division of two variables with independent, random uncertainties, the relative uncertainties are added exactly as they are in multiplication:

$$
\frac{\Delta R}{R} = \frac{\Delta V}{V} + \frac{\Delta I}{I}
$$

## Step-by-Step Solution
Calculate the central value for the resistance:

$$
\begin{align}
R &= \frac{10.0}{2.00} \\
  &= 5.00 \, \Omega
\end{align}
$$

Calculate the total relative uncertainty:

$$
\begin{align}
\frac{\Delta R}{R} &= \frac{0.2}{10.0} + \frac{0.05}{2.00} \\
                   &= 0.02 + 0.025 \\
                   &= 0.045
\end{align}
$$

Calculate the absolute uncertainty $\Delta R$:

$$
\begin{align}
\Delta R &= R \cdot (\frac{\Delta V}{V} + \frac{\Delta I}{I}) \\
         &= 5.00 \cdot 0.045 \\
         &= 0.225 \, \Omega
\end{align}
$$

Rounding to a reasonable standard of precision (one or two significant figures for error):

## Final Result

$$
R = (5.00 \pm 0.23) \, \Omega
$$

## Interpretation
The calculated resistance is $5.00 \, \Omega$ with an uncertainty of $0.23 \, \Omega$. Both instruments contribute similarly to the total error, with the current measurement introducing slightly more percentage uncertainty ($2.5\%$) compared to the voltage measurement ($2.0\%$).