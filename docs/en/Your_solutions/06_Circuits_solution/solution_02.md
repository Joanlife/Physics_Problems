# Task 02 – Combinations of Three Resistors

## Problem Statement
Given exactly three $1\,\Omega$ resistors, determine all unique possible equivalent resistances that can be created by combining them in any configuration.

## Theory
Resistors can be combined in series ($R_1 + R_2$) or parallel ($\frac{R_1 R_2}{R_1 + R_2}$). With three resistors, the following topologies are possible:
1. All in series.
2. All in parallel.
3. Two in series, then parallel with the third.
4. Two in parallel, then series with the third.

## Step-by-Step Solution

### Configuration 1: All in Series
All three resistors are in a single line.

$$
R_{eq} = 1 + 1 + 1 = 3\,\Omega
$$

### Configuration 2: All in Parallel
All three resistors share the same two nodes.

$$
\frac{1}{R_{eq}} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 3 \implies R_{eq} = \frac{1}{3}\,\Omega \approx 0.33\,\Omega
$$

### Configuration 3: Two in Series, Parallel with One
$R_1$ and $R_2$ are in series ($2\,\Omega$), and this branch is parallel to $R_3$ ($1\,\Omega$).

$$
R_{eq} = \frac{2 \cdot 1}{2 + 1} = \frac{2}{3}\,\Omega \approx 0.67\,\Omega
$$

### Configuration 4: Two in Parallel, Series with One
$R_1$ and $R_2$ are in parallel ($0.5\,\Omega$), and this combination is in series with $R_3$ ($1\,\Omega$).

$$
R_{eq} = \frac{1 \cdot 1}{1 + 1} + 1 = 0.5 + 1 = 1.5\,\Omega
$$

## Final Result
The unique equivalent resistances are:
- $3\,\Omega$
- $1.5\,\Omega$
- $0.67\,\Omega$
- $0.33\,\Omega$

## Interpretation
Changing the topology of the circuit allows for a wide range of resistance values (from $1/3$ to 3 times the base resistance) using the same components.