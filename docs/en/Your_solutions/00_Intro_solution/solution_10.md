# Task 10 – Infinite Series

## Problem Statement

An ant moves according to the pattern:

1 m east,  
1/2 m north,  
1/3 m west,  
1/4 m south,  
1/5 m east, and so on.

Determine its final position.

---

## Theory

The motion separates into two alternating infinite series: one horizontal and one vertical.

---

## Step-by-Step Solution

Horizontal displacement:

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots
$$

This series is known:

$$
\sum_{k=0}^{\infty}\frac{(-1)^k}{2k+1} = \frac{\pi}{4}
$$

Vertical displacement:

$$
\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots
$$

This series equals

$$
\frac{1}{2}\ln 2
$$

---

## Final Result

Final coordinates:

$$
x = \frac{\pi}{4}
$$

$$
y = \frac{1}{2}\ln 2
$$

---

## Interpretation

Both series converge, so the ant approaches a fixed position despite infinitely many steps.