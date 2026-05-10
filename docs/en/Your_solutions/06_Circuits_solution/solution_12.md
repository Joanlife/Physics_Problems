# Task 12 – Transformer Calculations

## Problem Statement

A transformer has:
- Primary turns $N_p = 1000$
- Secondary turns $N_s = 200$
- Primary voltage $V_p = 120\,\text{V}$ (AC)
- Secondary current $I_s = 3\,\text{A}$

Find the secondary voltage ($V_s$) and the primary current ($I_p$).

## Theory

The Transformer Equation relates turns to voltage:

$$
\frac{V_s}{V_p} = \frac{N_s}{N_p}
$$

For an ideal transformer (100% efficient), power is conserved ($P_p = P_s$), leading to the current relationship:

$$
\frac{I_p}{I_s} = \frac{N_s}{N_p}
$$

## Step-by-Step Solution

### 1. Secondary Voltage
Rearranging the transformer equation:

$$
\begin{align}
V_s &= V_p \left( \frac{N_s}{N_p} \right) \\
    &= 120\,\text{V} \left( \frac{200}{1000} \right) \\
    &= 120 \cdot 0.2 = 24\,\text{V}
\end{align}
$$

### 2. Primary Current
Using the inverse relationship for current:

$$
\begin{align}
I_p &= I_s \left( \frac{N_s}{N_p} \right) \\
    &= 3\,\text{A} \left( \frac{200}{1000} \right) \\
    &= 3 \cdot 0.2 = 0.6\,\text{A}
\end{align}
$$

## Final Result

- **Secondary Voltage:** $24\,\text{V}$
- **Primary Current:** $0.6\,\text{A}$

## Interpretation
This is a **step-down transformer**. It reduces the voltage by a factor of 5, which causes the current on the primary side to be 5 times smaller than the current on the secondary side (maintaining power balance).