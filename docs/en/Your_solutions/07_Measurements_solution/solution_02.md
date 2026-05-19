# Task 02 – Propagation of Error II

## Problem Statement
The length and width of a rectangular plate are measured to be $L = (15.3 \pm 0.1)\text{ cm}$ and $W = (8.4 \pm 0.1)\text{ cm}$. Calculate the area of the plate and its uncertainty.

## Theory
The area of a rectangle is determined by the product of its length and width:

$$
A = L \cdot W
$$

According to product rule, when multiplying two variables with independent uncertainties, their fractional (or relative) uncertainties are added:

$$
\frac{\Delta A}{A} = \frac{\Delta L}{L} + \frac{\Delta W}{W}
$$

## Step-by-Step Solution
First, compute the central value for the area:

$$
\begin{align}
A &= 15.3 \cdot 8.4 \\
  &= 128.52 \text{ cm}^2
\end{align}
$$

Next, substitute the measured values into the relative uncertainty formula:

$$
\begin{align}
\frac{\Delta A}{A} &=  \frac{0.1}{15.3} + \frac{0.1}{8.4} \\
                   &\approx 0.00654 + 0.01190 \\
                   &\approx 0.01844
\end{align}
$$

Finally, isolate and calculate the absolute uncertainty $\Delta A$:

$$
\begin{align}
\Delta A &= A ( \frac{\Delta L}{L} + \frac{\Delta W}{W}) \\
         &= 128.52 \cdot 0.01844 \\
         &\approx 2.37 \text{ cm}^2
\end{align}
$$

## Final Result

$$
A = (128.5 \pm 2.4) \text{ cm}^2
$$

## Interpretation
The calculated area is $128.5 \text{ cm}^2$. It is notable that the width $W$ contributes more heavily to the final uncertainty than the length $L$, because $0.1 \text{ cm}$ represents a larger percentage error relative to $8.4 \text{ cm}$ than it does to $15.3 \text{ cm}$.