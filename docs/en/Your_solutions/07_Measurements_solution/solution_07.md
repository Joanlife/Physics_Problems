# Task 07 – Standard Deviation

## Problem Statement
Eleven students received the following test scores: 88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89. 
Calculate the mean and standard deviation. Then, remove the highest and lowest scores, and recalculate the new mean and standard deviation.

## Theory
The arithmetic mean $\bar{x}$ represents the central tendency of a dataset of $N$ values:

$$
\bar{x} = \frac{1}{N} \sum_{i=1}^N x_i
$$

The sample standard deviation $\sigma$ (or $s$) quantifies the dispersion of the dataset relative to the mean:

$$
\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^N (x_i - \bar{x})^2}
$$

## Step-by-Step Solution

### Part 1: Full Dataset ($N = 11$)
Data: $\{77, 79, 81, 83, 85, 86, 88, 89, 90, 92, 95\}$

Calculate the sum:

$$
\sum x_i = 945
$$

Calculate the mean:

$$
\begin{align}
\bar{x}_{11} &= \frac{945}{11} \\
             &\approx 85.91
\end{align}
$$

Calculate the sum of squared deviations $\sum (x_i - 85.91)^2$:

$$
\sum (x_i - \bar{x})^2 \approx 312.91
$$

Calculate standard deviation:

$$
\begin{align}
\sigma_{11} &= \sqrt{\frac{312.91}{11 - 1}} \\
            &= \sqrt{31.291} \\
            &\approx 5.59
\end{align}
$$

### Part 2: Truncated Dataset ($N = 9$)
Remove the highest ($95$) and lowest ($77$) scores.
New Data: $\{79, 81, 83, 85, 86, 88, 89, 90, 92\}$

Calculate the new sum:

$$
\sum x_i = 773
$$

Calculate the new mean:

$$
\begin{align}
\bar{x}_{9} &= \frac{773}{9} \\
            &\approx 85.89
\end{align}
$$

Calculate the new sum of squared deviations $\sum (x_i - 85.89)^2$:

$$
\sum (x_i - \bar{x})^2 \approx 150.89
$$

Calculate new standard deviation:

$$
\begin{align}
\sigma_{9} &= \sqrt{\frac{150.89}{9 - 1}} \\
           &= \sqrt{18.86} \\
           &\approx 4.34
\end{align}
$$

## Final Result

**Original Dataset:**

$$
\bar{x} = 85.91, \quad \sigma = 5.59
$$

**Truncated Dataset:**

$$
\bar{x} = 85.89, \quad \sigma = 4.34
$$

## Interpretation
Removing the outliers (highest and lowest scores) barely shifts the mean (from $85.91$ to $85.89$). However, the standard deviation drops significantly (from $5.59$ to $4.34$), proving that extreme values disproportionately inflate the standard deviation due to the squaring of their large distances from the mean.