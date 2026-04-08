# Task 09 – Damped Harmonic Oscillator

## Problem Statement

For the given equation describing a damped harmonic oscillator:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

1. Write down the general solution.
2. Present the classification of cases: underdamped, critically damped, overdamped.
3. Solve the equation numerically (RK4) and provide an interactive HTML animation.
4. Investigate the effect of parameter $b$.
5. Generate the graph of $x(t)$ and the phase portrait.

## Theory

The equation is a second-order linear homogeneous differential equation with constant coefficients. By dividing by $m$, we define:
* $\gamma = \frac{b}{2m}$ (damping coefficient)
* $\omega_0^2 = \frac{k}{m}$ (undamped natural frequency)

The characteristic equation is $r^2 + 2\gamma r + \omega_0^2 = 0$, with roots:

$$
r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

### Classification of Cases

1. **Underdamped ($\gamma < \omega_0$):** Roots are complex. The system oscillates with decaying amplitude.
2. **Critically Damped ($\gamma = \omega_0$):** Real repeated roots. The system returns to equilibrium fastest without oscillation.
3. **Overdamped ($\gamma > \omega_0$):** Real distinct roots. The system returns to equilibrium slowly.

## Step-by-Step Solution (Numerical)

To solve numerically using the 4th Order Runge-Kutta (RK4) method, we transform the 2nd order ODE into a system of two 1st order ODEs:

$$
\begin{align}
\frac{dx}{dt} &= v \\
\frac{dv}{dt} &= -\frac{b}{m}v - \frac{k}{m}x
\end{align}
$$

## Interactive Implementation

The following HTML code creates a simulation with a slider for the damping coefficient $b$.

```html
<!DOCTYPE html>
<html>
<head>
    <script src="[https://cdn.plot.ly/plotly-latest.min.js](https://cdn.plot.ly/plotly-latest.min.js)"></script>
    <style>
        body { font-family: sans-serif; display: flex; flex-direction: column; align-items: center; }
        .controls { margin: 20px; padding: 15px; border: 1px solid #ccc; border-radius: 8px; }
        #charts { display: flex; flex-wrap: wrap; justify-content: center; width: 100%; }
        .chart { width: 45%; min-width: 400px; height: 400px; }
    </style>
</head>
<body>
    <h2>Damped Harmonic Oscillator Simulation</h2>
    <div class="controls">
        <label>Damping (b): </label>
        <input type="range" id="bSlider" min="0" max="10" step="0.1" value="0.5">
        <span id="bVal">0.5</span>
    </div>
    <div id="charts">
        <div id="timeChart" class="chart"></div>
        <div id="phaseChart" class="chart"></div>
    </div>

    <script>
        const m = 1, k = 10;
        let b = 0.5;

        function rk4(x, v, dt, b) {
            const f1x = (x, v) => v;
            const f1v = (x, v) => -(b/m)*v - (k/m)*x;

            let k1x = dt * f1x(x, v);
            let k1v = dt * f1v(x, v);
            let k2x = dt * f1x(x + k1x/2, v + k1v/2);
            let k2v = dt * f1v(x + k1x/2, v + k1v/2);
            let k3x = dt * f1x(x + k2x/2, v + k2v/2);
            let k3v = dt * f1v(x + k2x/2, v + k2v/2);
            let k4x = dt * f1x(x + k3x, v + k3v);
            let k4v = dt * f1v(x + k3x, v + k3v);

            return {
                x: x + (k1x + 2*k2x + 2*k3x + k4x) / 6,
                v: v + (k1v + 2*k2v + 2*k3v + k4v) / 6
            };
        }

        function update() {
            let x = 2, v = 0, dt = 0.05;
            let times = [], xs = [], vs = [];
            for (let t = 0; t < 20; t += dt) {
                times.push(t); xs.push(x); vs.push(v);
                let next = rk4(x, v, dt, b);
                x = next.x; v = next.v;
            }

            Plotly.newPlot('timeChart', [{x: times, y: xs, name: 'Position x(t)'}], {title: 'Position vs Time'});
            Plotly.newPlot('phaseChart', [{x: xs, y: vs, name: 'Phase Portrait'}], {title: 'Velocity vs Position', xaxis: {title: 'x'}, yaxis: {title: 'v'}});
        }

        document.getElementById('bSlider').oninput = function() {
            b = parseFloat(this.value);
            document.getElementById('bVal').innerText = b;
            update();
        };
        update();
    </script>
</body>
</html>