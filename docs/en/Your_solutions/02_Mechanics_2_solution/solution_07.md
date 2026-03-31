# Task 07 – Dynamics with Friction: Multi-Block System

## Problem Statement

A $5\text{ kg}$ block (Block 1) is placed on a $10\text{ kg}$ block (Block 2). A horizontal force of $45\text{ N}$ is applied to the $10\text{ kg}$ block, and the $5\text{ kg}$ block is tied to the wall. The coefficient of kinetic friction $\mu_k$ between all moving surfaces is $0.2$. Find the acceleration of the $10\text{ kg}$ block.

## Theory

This is a dynamics problem involving Newton's Second Law because we are dealing with unbalanced forces that result in acceleration: 

$$
\sum F = ma
$$

For the $10\text{ kg}$ block (Block 2) to move, it must overcome two frictional forces:
1. Friction from the ground acting on the bottom of Block 2.
2. Friction from the $5\text{ kg}$ block (Block 1) acting on the top of Block 2.

The kinetic friction force is defined as $F_f = \mu_k N$, where $N$ is the normal force.

## Step-by-Step Solution

### 1. Identify Normal Forces

* **Normal force on Block 1 ($N_1$):** Produced by its own weight.
  $$N_1 = m_1 g = 5 \cdot 9.81 = 49.05\text{ N}$$
* **Normal force on Block 2 ($N_2$):** Produced by the combined weight of both blocks pressing on the ground.
  $$N_2 = (m_1 + m_2)g = (5 + 10) \cdot 9.81 = 147.15\text{ N}$$

### 2. Calculate Frictional Forces

* **Friction between Block 1 and Block 2 ($F_{f1}$):**
  $$F_{f1} = \mu_k N_1 = 0.2 \cdot 49.05 = 9.81\text{ N}$$
* **Friction between Block 2 and the ground ($F_{f2}$):**
  $$F_{f2} = \mu_k N_2 = 0.2 \cdot 147.15 = 29.43\text{ N}$$

### 3. Equation of Motion for Block 2

Block 2 is pulled by $F = 45\text{ N}$. It is resisted by both friction forces $F_{f1}$ (top) and $F_{f2}$ (bottom).

$$
F - F_{f1} - F_{f2} = m_2 a
$$

$$
45 - 9.81 - 29.43 = 10 \cdot a
$$

$$
45 - 39.24 = 10a
$$

$$
5.76 = 10a \implies a = 0.576\text{ m/s}^2
$$

## Final Result

The acceleration of the $10\text{ kg}$ block is $0.576\text{ m/s}^2$.

## Interpretation

Even though a $45\text{ N}$ force is applied, nearly $87\%$ of that force is "wasted" overcoming friction. Because the top block is tied to the wall, it remains stationary, exerting a constant frictional drag on the moving block below it.