# Task 08 – AC Voltage Equation

## Problem Statement

The current in an AC circuit is given by the function $I(t) = 2 \sin(120\pi t)$. If the circuit consists of a single $50\,\Omega$ resistor, determine the equation for the voltage $V(t)$ across it.

## Theory

### Ohm's Law in AC Circuits
For a purely resistive circuit, Ohm's Law applies to the instantaneous values of voltage and current just as it does in DC circuits. The relationship is:

$$
V(t) = I(t) \cdot R
$$




## Step-by-Step Solution


### 1. Apply Ohm's Law
Substitute the current function into the Ohm's Law equation:

$$
\begin{align}
V(t) &= [2 \sin(120\pi t)] \cdot 50 \\
V(t) &= (2 \cdot 50) \cdot \sin(120\pi t)
\end{align}
$$

### 2. Simplify the Equation
Perform the multiplication to find the peak voltage ($V_{max}$):

$$
V(t) = 100 \sin(120\pi t)
$$

## Final Result

$$
V(t) = 100 \sin(120\pi t)
$$

## Interpretation
The resulting voltage has a peak value of $100\,\text{V}$. Because the load is purely resistive, the voltage follows the exact same frequency ($60\,\text{Hz}$, derived from $120\pi/2\pi$) and phase as the current. 