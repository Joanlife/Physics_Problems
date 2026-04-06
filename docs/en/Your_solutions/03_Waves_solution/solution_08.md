# Task 08 – Wave Equation Verification

## Problem Statement

Which of the following functions can describe a traveling wave? Hint: check if it satisfies the wave equation:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

a) $y(x,t) = A \cos(kx^2 - \omega t)$
b) $y(x,t) = A(x-vt)^2$
c) $y(x,t) = A \log(x+vt)$

## Theory

Any function that represents a traveling wave with a constant shape must be of the form $f(x \pm vt)$. A more rigorous test is the linear wave equation shown above. If a function satisfies this second-order partial differential equation, it is a valid wave.

## Step-by-Step Solution

### Case (a): $y = A \cos(kx^2 - \omega t)$
Let's find the second derivatives:
* $\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot 2kx$
* $\frac{\partial^2 y}{\partial x^2}$ will involve terms with $x^2$ and constant terms (product rule), resulting in a non-linear relationship that does not simply scale with the time derivative.
* Function shape changes as it moves because of $x^2$.
**Result: NOT a traveling wave.**

### Case (b): $y = A(x-vt)^2$
Let $u = x-vt$. Then $y = Au^2$.
* $\frac{\partial y}{\partial x} = 2Au \frac{\partial u}{\partial x} = 2Au(1)$
* $\frac{\partial^2 y}{\partial x^2} = 2A$
* $\frac{\partial y}{\partial t} = 2Au \frac{\partial u}{\partial t} = 2Au(-v) = -2Auv$
* $\frac{\partial^2 y}{\partial t^2} = -2Av \frac{\partial u}{\partial t} = -2Av(-v) = 2Av^2$

Test the wave equation:

$$
2A = \frac{1}{v^2} (2Av^2) \implies 2A = 2A
$$

**Result: IS a traveling wave.**

### Case (c): $y = A \log(x+vt)$
Following the same logic, since this is in the form $f(x+vt)$:
* $\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}$
* $\frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}$

Test the wave equation:

$$
-\frac{A}{(x+vt)^2} = \frac{1}{v^2} \left( -\frac{Av^2}{(x+vt)^2} \right)
$$

**Result: IS a traveling wave.**

## Final Result

Functions **(b)** and **(c)** describe traveling waves. Function **(a)** does not.

## Interpretation

Functions of the form $f(x \pm vt)$ satisfy the wave equation regardless of the specific shape of $f$ (be it a square, a log, or a parabola), provided the function is twice differentiable. Function (a) fails because the spatial part $kx^2$ prevents the wave from maintaining a constant shape as it translates.