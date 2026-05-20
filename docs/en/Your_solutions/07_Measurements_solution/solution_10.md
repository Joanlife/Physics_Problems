# Task 10 – Light Speed Measurement

## Problem Statement
Measure the speed of light using a microwave oven, a bar of chocolate, and a ruler. Measure the distance between melted spots to determine the wavelength. Use the microwave's frequency $f=2.45\text{ GHz}$ to calculate the speed of light, compare it to the accepted value of $c = 300,000,000\text{ m/s}$, and determine the percentage error.

## Theory
Electromagnetic waves, including microwaves, travel at the speed of light $c$. The wave speed is the product of its wavelength $\lambda$ and frequency $f$:

$$
c = \lambda f
$$

Inside a microwave oven, waves reflect off the metal walls and interfere to form a standing wave. The intense heating points that melt the chocolate correspond to the antinodes (points of maximum amplitude) of this standing wave. The distance $d$ between two adjacent antinodes is exactly half of one wavelength:

$$
d = \frac{\lambda}{2}
$$

By rearranging this, the wavelength is defined as $\lambda = 2d$. The experimental speed of light $c_{exp}$ becomes:

$$
c_{exp} = 2 d f
$$

To evaluate the accuracy of the experiment, the percentage error compares the measured value to the theoretical accepted value $c_{true}$:

$$
\text{Percentage Error} = \left| \frac{c_{exp} - c_{true}}{c_{true}} \right| \cdot 100\%
$$

## Step-by-Step Solution
*(Note: As this is a physical experiment, the steps below outline the strict mathematical procedure required to process the data once the distance $d$ is physically measured.)*

1. **Record the Distance:** Measure the distance $d$ between the geometric centers of two adjacent melted spots on the chocolate. Convert this measurement to meters (e.g., $6.0\text{ cm} = 0.06\text{ m}$).
2. **Calculate Wavelength:** Multiply the measured distance by two to find the full wavelength:

$$
\lambda = 2d
$$

3. **Convert Frequency:** Ensure the frequency is in standard SI units (Hertz) to yield a velocity in meters per second:

$$
f = 2.45 \text{ GHz} = 2.45 \times 10^9 \text{ Hz}
$$

4. **Calculate Experimental Speed:** Multiply the calculated wavelength by the frequency:

$$
c_{exp} = \lambda \cdot (2.45 \times 10^9)
$$

5. **Calculate Percentage Error:** Substitute the calculated $c_{exp}$ and the accepted speed $c_{true} = 3 \times 10^8 \text{ m/s}$ into the percentage error formula:

$$
\text{Percentage Error} = \left| \frac{c_{exp} - 300000000}{300000000} \right| \cdot 100\%
$$

## Final Result
The final processed data will take the form:

$$
c_{exp} = [ \text{Calculated Value} ] \text{ m/s}
$$

$$
\text{Percentage Error} = [ \text{Calculated} ] \%
$$

## Interpretation
Because the frequency of a commercial microwave is heavily regulated and highly stable, the primary source of error in this experiment stems from measuring the distance $d$. The melted chocolate regions are often wide and irregular, making it difficult to locate their exact centers. Despite this mechanical limitation, the standing wave pattern provides a surprisingly accurate macroscopic demonstration of an invisible quantum property.