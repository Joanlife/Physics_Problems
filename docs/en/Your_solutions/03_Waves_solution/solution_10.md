# Task 10 – Animation: Wave Sources

## Problem Statement

Write an HTML animation in which it is possible to place dots that serve as sources of waves described by:

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r_0}|^\alpha} \sin(k |\vec{r} - \vec{r_0}| - \omega t)
$$

Include a parameter $\alpha \in [0, 2]$ and show the superposition of waves from all dots.

## Theory

This equation describes a wave emanating from a point source located at $\vec{r_0}$. The parameter $\alpha$ determines the spatial attenuation (damping) of the wave:
* $\alpha = 0$: Plane-like wave with no amplitude decay.
* $\alpha = 0.5$: Cylindrical wave decay.
* $\alpha = 1.0$: Spherical wave decay (inverse distance law).

The total displacement $U$ at any point is the sum of the individual wave contributions from each source $i$:

$$
U(\vec{r}, t) = \sum_{i} u_i(\vec{r}, t)
$$

## Step-by-Step Solution



The implementation uses a 2D canvas context. For every frame, the script calculates the distance from each pixel to every source, computes the phase, and updates the pixel intensity.

```html
<!DOCTYPE html>
<html>
<body style="background:#000; color:#fff; font-family:sans-serif;">
    <h3>Wave Source Superposition</h3>
    <canvas id="waveCanvas" width="600" height="400" style="background:black; cursor: crosshair; border:1px solid #444;"></canvas>
    <div style="margin-top:10px;">
        Attenuation (α): <input type="range" id="alpha" min="0" max="2" step="0.1" value="0.5">
        <p>Click the canvas to add wave sources.</p>
    </div>

    <script>
        const canvas = document.getElementById('waveCanvas');
        const ctx = canvas.getContext('2d');
        const sources = [];
        let time = 0;

        canvas.onclick = (e) => {
            const rect = canvas.getBoundingClientRect();
            sources.push({x: e.clientX - rect.left, y: e.clientY - rect.top});
        };

        function draw() {
            const alpha = parseFloat(document.getElementById('alpha').value);
            const imgData = ctx.createImageData(canvas.width, canvas.height);
            const data = imgData.data;

            for (let y = 0; y < canvas.height; y += 2) {
                for (let x = 0; x < canvas.width; x += 2) {
                    let totalU = 0;
                    sources.forEach(s => {
                        const dist = Math.sqrt((x-s.x)**2 + (y-s.y)**2) + 1;
                        totalU += (25 / Math.pow(dist, alpha)) * Math.sin(0.2 * dist - time);
                    });

                    const val = 128 + totalU * 10;
                    const idx = (y * canvas.width + x) * 4;
                    // Grayscale mapping
                    data[idx] = data[idx+1] = data[idx+2] = val;
                    data[idx+3] = 255;
                    
                    // 2x2 block fill for performance
                    const nextIdx = (y * canvas.width + (x+1)) * 4;
                    data[nextIdx] = data[nextIdx+1] = data[nextIdx+2] = val;
                    data[nextIdx+3] = 255;
                }
            }
            ctx.putImageData(imgData, 0, 0);
            time += 0.15;
            requestAnimationFrame(draw);
        }
        draw();
    </script>
</body>
</html>