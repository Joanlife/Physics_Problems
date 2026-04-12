# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with a velocity $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \text{ m/s}$ in a region where the magnetic field is $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \text{ T}$. What is the magnitude of the magnetic force this charge experiences?

## Theory

When velocity and magnetic field are given in vector components, we use the determinant method for the cross product:
$$
\vec{F} = q (\vec{v} \times \vec{B})
$$

The charge of a proton is $q \approx 1.6 \times 10^{-19} \text{ C}$.

## Step-by-Step Solution

### 1. Calculate the Cross Product $(\vec{v} \times \vec{B})$
$$
\vec{v} \times \vec{B} = 
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

Calculating the components:
- $\hat{i}: (-4)(-1) - (1)(2) = 4 - 2 = 2$
- $\hat{j}: -[(2)(-1) - (1)(1)] = -[-2 - 1] = 3$
- $\hat{k}: (2)(2) - (-4)(1) = 4 + 4 = 8$

So, $\vec{v} \times \vec{B} = (2\hat{i} + 3\hat{j} + 8\hat{k})$.

### 2. Calculate the Magnitude of the Vector
$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2} = \sqrt{4 + 9 + 64} = \sqrt{77} \approx 8.775
$$

### 3. Apply the Charge
$$
F = q |\vec{v} \times \vec{B}| = (1.6 \times 10^{-19}) \cdot 8.775
$$

$$
F \approx 1.40 \times 10^{-18} \text{ N}
$$

## Final Result

The magnitude of the magnetic force is:
$$
F \approx 1.40 \times 10^{-18} \text{ N}
$$

## Interpretation

In three-dimensional space, the force is always perpendicular to both the velocity and the magnetic field. This vector approach is essential when the movement is not neatly perpendicular to the field lines.