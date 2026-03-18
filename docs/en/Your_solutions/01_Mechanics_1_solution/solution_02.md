# Task 02 – Range Optimization

## Problem Statement
Show analytically that the maximum range $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

## Theory
The range of a projectile on level ground is a function of the launch angle $\theta$. To find the maximum of a function, we must find the derivative with respect to the independent variable and set it to zero.

## Step-by-Step Solution

We start with the range equation:

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

To find the extremum, we calculate $\frac{dR}{d\theta}$:

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \frac{d}{d\theta}(\sin(2\theta))
$$

Using the chain rule:

$$
\frac{dR}{d\theta} = \frac{2v_0^2}{g} \cos(2\theta)
$$

To find the angle for maximum range,we set the first derivative to zero;


$$
\frac{2v_0^2}{g} \cos(2\theta) = 0
$$

Since $v_0$ and $g$ are non-zero constants:

$$
\cos(2\theta) = 0
$$

For the physical domain of projectile motion ($0 < \theta < \pi/2$), this occurs when:

$$
2\theta = 90^\circ \implies \theta = 45^\circ
$$

To confirm it is a maximum, we check the second derivative:

$$
\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(2\theta)
$$

At $\theta = 45^\circ$, $\sin(90^\circ) = 1$, so the second derivative is negative, confirming a local maximum.

## Final Result
The maximum range is achieved at $\theta = 45^\circ$.

## Interpretation
At $45^\circ$, the projectile balances the trade-off between vertical "hang time" and horizontal velocity components optimally.