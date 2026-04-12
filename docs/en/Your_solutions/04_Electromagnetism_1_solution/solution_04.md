# Task 04 – Force Comparison: Electric vs. Gravitational

## Problem Statement

Calculate the magnitude of the electric force and the gravitational force between an electron and a proton in a hydrogen atom (average distance $r \approx 5.3 \times 10^{-11}$ m). What is the ratio $F_e/F_g$?

## Theory

To compare these forces, we use **Coulomb's Law** for the electric force and **Newton's Law of Universal Gravitation** for the gravitational force:

$$
F_e = k \frac{|q_e q_p|}{r^2}
$$

$$
F_g = G \frac{m_e m_p}{r^2}
$$

**Constants:**
- $k \approx 8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$
- $G \approx 6.67 \times 10^{-11} \text{ N}\cdot\text{m}^2/\text{kg}^2$
- $q_e = q_p \approx 1.60 \times 10^{-19} \text{ C}$
- $m_e \approx 9.11 \times 10^{-31} \text{ kg}$
- $m_p \approx 1.67 \times 10^{-27} \text{ kg}$

## Step-by-Step Solution

### 1. Electric Force ($F_e$)
Substitute the values into Coulomb's equation:

$$
F_e = (8.99 \times 10^9) \frac{(1.60 \times 10^{-19})^2}{(5.3 \times 10^{-11})^2}
$$

$$
F_e \approx 8.2 \times 10^{-8} \text{ N}
$$

### 2. Gravitational Force ($F_g$)
Substitute the values into Newton's equation:

$$
F_g = (6.67 \times 10^{-11}) \frac{(9.11 \times 10^{-31})(1.67 \times 10^{-27})}{(5.3 \times 10^{-11})^2}
$$

$$
F_g \approx 3.6 \times 10^{-47} \text{ N}
$$

### 3. Calculating the Ratio
Since both forces depend on $1/r^2$, the distance cancels out when we divide them:

$$
\frac{F_e}{F_g} = \frac{k |q_e q_p|}{G m_e m_p}
$$

$$
\frac{F_e}{F_g} \approx \frac{8.2 \times 10^{-8}}{3.6 \times 10^{-47}} \approx 2.27 \times 10^{39}
$$

## Final Result

- **Electric Force:** $F_e \approx 8.2 \times 10^{-8} \text{ N}$
- **Gravitational Force:** $F_g \approx 3.6 \times 10^{-47} \text{ N}$
- **Ratio:** $F_e/F_g \approx 2.3 \times 10^{39}$

## Interpretation

The electric force is approximately $10^{39}$ times stronger than the gravitational force. In the context of atomic physics, gravity is so weak that it is effectively non-existent. This is why chemical bonds and atomic structures are governed entirely by electromagnetic interactions rather than gravity.