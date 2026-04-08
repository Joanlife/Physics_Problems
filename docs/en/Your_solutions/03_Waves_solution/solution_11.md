# Task 11 – Animation: Two-Slit Interference

## Problem Statement

Write an HTML animation simulating Young's experiment. Two slits act as point sources of coherent waves. The displacement of the resultant wave is the sum of partial waves described by the formula:

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_1}|} \sin(k |\vec{r} - \vec{r_1}| - \omega t) + \frac{A}{|\vec{r}-\vec{r_2}|} \sin(k |\vec{r} - \vec{r_2}| - \omega t)
$$

where $\vec{r_1}$ and $\vec{r_2}$ are the position vectors of the slits. The user should be able to change the distance between the slits $d = |\vec{r_1} - \vec{r_2}|$ and the wavelength $\lambda$. The animation should visualize the resulting interference pattern in real time.

## Theory

Young's double-slit experiment is a classic demonstration of the wave nature of light and the principle of **superposition**. When two coherent wave sources overlap, they interfere.



[Image of Young's double-slit interference pattern]


The nature of the interference at any point $\vec{r}$ depends on the **path difference** $\Delta L = |d_1 - d_2|$:

1.  **Constructive Interference:** Occurs when $\Delta L = n\lambda$ (where $n$ is an integer). The waves arrive in phase, creating a maximum (bright fringe).
2.  **Destructive Interference:** Occurs when $\Delta L = (n + \frac{1}{2})\lambda$. The waves arrive $180^\circ$ out of phase, creating a minimum (dark fringe).

The angular spacing of these fringes is governed by the relation:

$$
d \sin(\theta) = n\lambda
$$

## Step-by-Step Solution

The implementation uses the HTML5 Canvas API to calculate the wave amplitude at every pixel on a grid. We map the calculated displacement $u(\vec{r},t)$ to a color value to visualize the wavefronts.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Young's Interference Simulation</title>
    <style>
        body { background: #000; color: #eee; font-family: sans-serif; text-align: center; }
        canvas { border: 1px solid #444; background: #000; cursor: crosshair; }
        .controls { margin: 20px; padding: 15px; background: #222; display: inline-block; border-radius: 10px; }
        label { margin-right: 10px; }
    </style>
</head>
<body>
    <h2>Two-Slit Interference Animation</h2>
    <canvas id="canvas" width="600" height="400"></canvas>
    <div class="controls">
        <label>Slit Distance (d):</label>
        <input type="range" id="dSlider" min="10" max="150" value="40">
        <label>Wavelength (λ):</label>
        <input type="range" id="lSlider" min="10" max="60" value="25">
    </div>

    <script>
        const canvas = document.getElementById('canvas');
        const ctx = canvas.getContext('2d');
        const dSlider = document.getElementById('dSlider');
        const lSlider = document.getElementById('lSlider');

        let time = 0;

        function animate() {
            const d = parseInt(dSlider.value);
            const wavelength = parseInt(lSlider.value);
            const k = (2 * Math.PI) / wavelength;
            const omega = 0.2;
            
            const width = canvas.width;
            const height = canvas.height;
            const imgData = ctx.createImageData(width, height);
            const data = imgData.data;

            // Slit positions
            const s1y = height / 2 - d / 2;
            const s2y = height / 2 + d / 2;
            const sx = 40;

            for (let y = 0; y < height; y += 2) {
                for (let x = 0; x < width; x += 2) {
                    const d1 = Math.sqrt((x - sx) ** 2 + (y - s1y) ** 2);
                    const d2 = Math.sqrt((x - sx) ** 2 + (y - s2y) ** 2);

                    // Calculating the superposition
                    const u1 = (1 / (d1 / 20 + 1)) * Math.sin(k * d1 - time);
                    const u2 = (1 / (d2 / 20 + 1)) * Math.sin(k * d2 - time);
                    const totalU = u1 + u2;

                    // Map [-2, 2] to [0, 255] for visualization
                    const color = 128 + totalU * 60;
                    
                    for (let dy = 0; dy < 2; dy++) {
                        for (let dx = 0; dx < 2; dx++) {
                            const index = ((y + dy) * width + (x + dx)) * 4;
                            data[index] = color * 0.5;     // Red
                            data[index + 1] = color;       // Green
                            data[index + 2] = color * 0.9; // Blue
                            data[index + 3] = 255;         // Alpha
                        }
                    }
                }
            }

            ctx.putImageData(imgData, 0, 0);
            time += omega;
            requestAnimationFrame(animate);
        }

        animate();
    </script>
</body>
</html>