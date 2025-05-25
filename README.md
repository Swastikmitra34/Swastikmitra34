<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Swastik Mitra | AI | Math | Quantum | Quant</title>
  <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
  <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #0e0e0e;
      color: #e0e0e0;
      padding: 2rem;
      line-height: 1.6;
    }
    header {
      text-align: center;
      padding: 2rem 0;
    }
    h1 {
      font-size: 2.5rem;
      color: #00ffe1;
    }
    section {
      margin-bottom: 4rem;
    }
    .equation {
      background: #1e1e1e;
      padding: 1rem;
      border-radius: 8px;
      margin: 1rem 0;
    }
    .visual-description {
      background: #222;
      padding: 1rem;
      border-left: 4px solid #00ffe1;
      margin: 1rem 0;
    }
    .interactive-block {
      background: #333;
      padding: 1rem;
      border-radius: 8px;
      margin-top: 1rem;
    }
    canvas {
      width: 100%;
      height: 200px;
      background: #111;
    }
  </style>
</head>
<body>
  <header>
    <h1>Swastik Mitra | AI • Mathematics • Quantum Computing • Quant Research</h1>
    <p>Exploring Intelligence, Abstractions, and Markets through Equations and Imagination</p>
  </header>

  <section>
    <h2>Artificial Intelligence (Diffusion Models)</h2>
    <div class="equation">
      $$ \frac{d\mathbf{x}}{dt} = f(\mathbf{x}, t) + g(t) \cdot \mathbf{w}(t) $$
    </div>
    <div class="visual-description">
      This stochastic differential equation models the forward diffusion process, where noise is gradually added. In reverse, a neural network learns to denoise and generate realistic images or videos — the core idea behind text-to-video generation.
    </div>
    <div class="interactive-block">
      <p>🧠 Interactive Visual: Animate diffusion-noise buildup</p>
      <canvas id="diffusionCanvas"></canvas>
    </div>
  </section>

  <section>
    <h2>Pure Mathematics</h2>
    <div class="equation">
      $$ \int_0^\infty \frac{\sin x}{x} dx = \frac{\pi}{2} $$
    </div>
    <div class="visual-description">
      A foundational result in harmonic analysis. Signals, randomness, and quantum behaviors are tied to such elegant identities.
    </div>
    <div class="interactive-block">
      <p>📐 Interactive Plot: Explore convergence of integrals</p>
    </div>
  </section>

  <section>
    <h2>Quantum Computing</h2>
    <div class="equation">
      $$ |\psi\rangle = \alpha |0\rangle + \beta |1\rangle,\quad |\alpha|^2 + |\beta|^2 = 1 $$
    </div>
    <div class="visual-description">
      This quantum bit (qubit) encodes superposition — the cornerstone of quantum parallelism and computation.
    </div>
    <div class="interactive-block">
      <p>🌀 Interactive: Bloch sphere visualization coming soon...</p>
    </div>
  </section>

  <section>
    <h2>Quantitative Finance</h2>
    <div class="equation">
      $$ dS_t = \mu S_t dt + \sigma S_t dW_t $$
    </div>
    <div class="visual-description">
      The Black-Scholes model describes how asset prices evolve with drift \( \mu \) and volatility \( \sigma \), driven by Brownian motion \( dW_t \).
    </div>
    <div class="interactive-block">
      <p>📊 Interactive: Simulate stock paths using Geometric Brownian Motion</p>
    </div>
  </section>

  <footer style="text-align:center; padding:2rem; font-size:0.9rem; color:#777;">
    © 2025 Swastik Mitra | Crafted with Math, Code & Vision.
  </footer>

  <script>
    // Basic placeholder for interactive canvas (AI diffusion simulation sketch)
    const canvas = document.getElementById('diffusionCanvas');
    const ctx = canvas.getContext('2d');
    canvas.width = canvas.offsetWidth;
    canvas.height = canvas.offsetHeight;
    let t = 0;
    function draw() {
      ctx.fillStyle = 'rgba(0, 255, 225, 0.05)';
      for (let i = 0; i < 50; i++) {
        const x = Math.random() * canvas.width;
        const y = Math.random() * canvas.height;
        ctx.beginPath();
        ctx.arc(x, y, 1.5, 0, Math.PI * 2);
        ctx.fill();
      }
      t += 0.01;
      requestAnimationFrame(draw);
    }
    draw();
  </script>
</body>
</html>

