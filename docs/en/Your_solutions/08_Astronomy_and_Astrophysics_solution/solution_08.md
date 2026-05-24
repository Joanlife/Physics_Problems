# Task 08 – Interplanetary Travel

## Problem Statement

How much time would it take to travel or transmit information from Earth to Mars when the planets are at their closest approach (distance $d = 55\,\text{million kilometers} = 55 \times 10^6\,\text{km}$)?

Calculate the time for:
* a) A communications message sent at the speed of light ($c \approx 3.00 \times 10^8$ m/s).
* b) A spacecraft traveling at a constant speed of $40000$ km/h ($11.11$ km/s).
* c) A commercial airplane traveling at a constant speed of $900$ km/h.

## Theory

The duration $t$ required to traverse a linear distance $d$ at a constant velocity $v$ is modeled by the fundamental kinematic relation

$$
t = \frac{d}{v}
$$

To maintain mathematical consistency, all initial variables must be standard aligned before running calculation steps.

## Step-by-Step Solution

Convert the baseline distance parameter into standard meters and kilometers

$$
d = 55 \times 10^6\,\text{km} = 5.5 \times 10^{10}\,\text{m}
$$

### Part a) Electromagnetic Message at Speed of Light

The speed of light constant is $c = 3.00 \times 10^8\,\text{m/s}$.

$$
t_a = \frac{5.5 \times 10^{10}\,\text{m}}{3.00 \times 10^8\,\text{m/s}} \approx 183.33\,\text{s}
$$

Convert this duration into minutes

$$
t_a = \frac{183.33}{60} \approx 3.06\,\text{minutes}
$$

### Part b) Spacecraft at Velocity 40,000 km/h

The travel speed is given as $v_b = 40000\,\text{km/h} = 11.11\,\text{km/s}$. Using standard units with kilometer dimensions

$$
t_b = \frac{55 \times 10^6\,\text{km}}{40000\,\text{km/h}} = 1375\,\text{hours}
$$



### Part c) Commercial Aircraft at Velocity 900 km/h

The travel velocity is $v_c = 900\,\text{km/h}$.

$$
t_c = \frac{55 \times 10^6\,\text{km}}{900\,\text{km/h}} \approx 61111.11\,\text{hours}
$$

Convert this long period into days and years

$$
t_{\text{c, days}} = \frac{61111.11}{24} \approx 2546.30\,\text{days}
$$



## Final Result

At closest approach, the travel durations to Mars are:
* **Speed of light message:** $\approx 3.06\,\text{minutes}$ ($183.3\,\text{s}$)
* **Fast interplanetary spacecraft:** $\approx1375\,\text{hours}$
* **Commercial aircraft flight:** $\approx2546.3\,\text{days}$

## Interpretation

These figures highlight the challenges of interplanetary coordination. The three-minute light speed delay means real-time remote control of Mars rovers from Earth is physically impossible, requiring onboard autonomous landing systems. For human transport, a 57-day transit represents a highly optimized ballistic flight profile that is only possible when the two planets line up perfectly in their orbits, an alignment that occurs once every 26 months.