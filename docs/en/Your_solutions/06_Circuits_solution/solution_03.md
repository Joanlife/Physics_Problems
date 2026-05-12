# Task 03 – Mixed Circuit Analysis (I)

## Problem Statement

Calculate the equivalent resistance ($R_{eq}$) for the circuit shown in the figure (image-r1.png). All resistors in the network have a resistance value of $R = 5\ \Omega$.

## Theory

Mixed circuits consist of both series and parallel resistor combinations. To solve for the total resistance, we decompose the circuit into smaller sub-sections.

### Parallel Resistance
When resistors are in parallel, the reciprocal of the equivalent resistance is the sum of the reciprocals of each resistance:

$$
\frac{1}{R_p} = \frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}
$$

For two identical resistors ($R$), the parallel resistance is simply $R/2$.

### Series Resistance
When resistors are in series, the total resistance is the sum of the individual values:

$$
R_s = R_1 + R_2 + \dots + R_n
$$

## Step-by-Step Solution



### 1. Identify the Parallel Branch
The circuit features a central parallel block containing two resistors, $R_2$ and $R_3$. Since both are $5\ \Omega$:

$$
\begin{align}
\frac{1}{R_{23}} &= \frac{1}{5\ \Omega} + \frac{1}{5\ \Omega} \\
\frac{1}{R_{23}} &= \frac{2}{5\ \Omega} \\
R_{23} &= 2.5\ \Omega
\end{align}
$$

### 2. Combine the Remaining Series Resistors
The equivalent resistance of the parallel block ($R_{23}$) is now in series with the leading resistor ($R_1$) and the trailing resistor ($R_4$). 

$$
\begin{align}
R_{eq} &= R_1 + R_{23} + R_4 \\
R_{eq} &= 5\ \Omega + 2.5\ \Omega + 5\ \Omega \\
R_{eq} &= 12.5\ \Omega
\end{align}
$$

## Final Result

$$
R_{eq} = 12.5\ \Omega
$$

## Interpretation

In this configuration, the parallel segment reduces the total resistance relative to a purely series arrangement of the same components. The $2.5\ \Omega$ contribution from the parallel branch reflects how multiple paths for current decrease the overall opposition to flow compared to a single $5\ \Omega$ path.