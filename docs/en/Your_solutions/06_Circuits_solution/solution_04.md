# Task 04 – Mixed Circuit Analysis (II)

## Problem Statement

Calculate the equivalent resistance ($R_{eq}$) for the bridge circuit shown in the figure (image-r2.png). All resistors have a value of $R = 10\ \Omega$.

## Theory

The circuit shown is a **Wheatstone Bridge**. A bridge is "balanced" when the ratio of resistors in the two arms is equal, which is always the case when all resistors have the same value ($10\ \Omega$).



In a balanced bridge:
1. The potential difference across the central resistor is zero.
2. No current flows through the central branch.
3. The central resistor can be ignored for the calculation of equivalent resistance.

## Step-by-Step Solution

### 1. Check the Balance Condition
For a bridge with resistors $R_1, R_2$ (top) and $R_3, R_4$ (bottom):

$$
\frac{R_1}{R_2} = \frac{10}{10} = 1, \quad \frac{R_3}{R_4} = \frac{10}{10} = 1
$$

Since the ratios are equal, the bridge is balanced. We can treat the circuit as two parallel branches, each containing two $10\ \Omega$ resistors in series.

### 2. Calculate the Resistance of Each Branch
Upper branch ($R_{top}$):

$$
R_{top} = 10\ \Omega + 10\ \Omega = 20\ \Omega
$$

Lower branch ($R_{bottom}$):

$$
R_{bottom} = 10\ \Omega + 10\ \Omega = 20\ \Omega
$$

### 3. Calculate Total Equivalent Resistance
The two $20\ \Omega$ branches are in parallel:

$$
\begin{align}
\frac{1}{R_{eq}} &= \frac{1}{20\ \Omega} + \frac{1}{20\ \Omega} \\
\frac{1}{R_{eq}} &= \frac{2}{20\ \Omega} \\
\frac{1}{R_{eq}} &= \frac{1}{10\ \Omega}
\end{align}
$$

$$
R_{eq} = 10\ \Omega
$$

## Final Result

$$
R_{eq} = 10\ \Omega
$$

## Interpretation

In a symmetric network like a balanced Wheatstone bridge where all components are identical, the total resistance of the entire system is exactly equal to the resistance of a single component. The central resistor remains "electrically invisible" because it connects two points that are at the same electrical potential.