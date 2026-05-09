# Task 01 – Series and Parallel Circuits

## Problem Statement

Three resistors, $R_1 = 15\,\Omega$, $R_2 = 30\,\Omega$, and $R_3 = 50\,\Omega$, are connected to a $12\,\text{V}$ battery. Calculate the total equivalent resistance ($R_{eq}$) and the total current ($I_{tot}$) for two scenarios:
1. All resistors are connected in series.
2. All resistors are connected in parallel.

## Theory

### Series Connection
In a series circuit, the current has only one path to follow. The equivalent resistance is the algebraic sum of individual resistances:

$$
R_{eq} = \sum_{i=1}^{n} R_i = R_1 + R_2 + \dots + R_n
$$

### Parallel Connection
In a parallel circuit, the voltage across each resistor is the same. The reciprocal of the equivalent resistance is the sum of the reciprocals of the individual resistances:

$$
\frac{1}{R_{eq}} = \sum_{i=1}^{n} \frac{1}{R_i} = \frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}
$$

### Ohm's Law
The total current flowing from the battery is determined by the relationship:

$$
I_{tot} = \frac{V}{R_{eq}}
$$

## Step-by-Step Solution

### 1. Series Case
First, we calculate the equivalent resistance:

$$
\begin{align}
R_{eq,s} &= R_1 + R_2 + R_3 \\
         &= 15\,\Omega + 30\,\Omega + 50\,\Omega \\
         &= 95\,\Omega
\end{align}
$$

Next, we find the total current:

$$
\begin{align}
I_{tot,s} &= \frac{12\,\text{V}}{95\,\Omega} \\
          &\approx 0.1263\,\text{A}
\end{align}
$$

### 2. Parallel Case
First, we calculate the equivalent resistance:

$$
\begin{align}
\frac{1}{R_{eq,p}} &= \frac{1}{15} + \frac{1}{30} + \frac{1}{50} \\
                   &= \frac{10 + 5 + 3}{150} \\
                   &= \frac{18}{150}
\end{align}
$$

Inverting the fraction:

$$
R_{eq,p} = \frac{150}{18} \approx 8.33\,\Omega
$$

Next, we find the total current:

$$
\begin{align}
I_{tot,p} &= \frac{12\,\text{V}}{8.333\,\Omega} \\
          &= 1.44\,\text{A}
\end{align}
$$

## Final Result

- **Series:** $R_{eq} = 95\,\Omega$, $I_{tot} \approx 0.126\,\text{A}$
- **Parallel:** $R_{eq} \approx 8.33\,\Omega$, $I_{tot} = 1.44\,\text{A}$

## Interpretation
In a series circuit, the total resistance is always greater than the largest individual resistor, resulting in a lower current. In a parallel circuit, the total resistance is always smaller than the smallest individual resistor, leading to a significantly higher current draw from the source.