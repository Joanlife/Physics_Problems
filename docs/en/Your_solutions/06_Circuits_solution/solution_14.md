# Task 14 – RLC Circuits and Harmonic Oscillators

## Problem Statement

Write the differential equation for a series RLC circuit and compare it to the equation of a damped harmonic oscillator. Identify the analogies between electrical and mechanical terms.

## Theory

A series RLC circuit contains a resistor ($R$), inductor ($L$), and capacitor ($C$) connected to a voltage source $V(t)$. The sum of voltages across the components must equal the source voltage.

## Step-by-Step Solution

### 1. The RLC Differential Equation
Using Kirchhoff's Loop Law:

$$
V_L + V_R + V_C = V(t)
$$

Substituting the definitions $V_L = L \frac{dI}{dt}$, $V_R = IR$, and $I = \frac{dQ}{dt}$:

$$
L \frac{d^2Q}{dt^2} + R \frac{dQ}{dt} + \frac{1}{C}Q = V(t)
$$

### 2. The Damped Harmonic Oscillator Equation
For a mass $m$ on a spring with constant $k$ and damping $b$:

$$
m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F(t)
$$

### 3. Identifying Analogies

| Electrical Term | Mechanical Analogue |
| :--- | :--- |
| Inductance ($L$) | Mass ($m$) |
| Resistance ($R$) | Damping coefficient ($b$) |
| Reciprocal Capacitance ($1/C$) | Spring constant ($k$) |
| Charge ($Q$) | Displacement ($x$) |
| Voltage ($V$) | Force ($F$) |

## Final Result

The RLC circuit is mathematically identical to a mechanical damped oscillator, where $L$ provides "inertia" (resistance to change in current) and $1/C$ provides "stiffness."

## Interpretation
This analogy allows engineers to model mechanical systems using electrical circuits and vice versa, as the underlying physics of energy exchange and dissipation is the same.