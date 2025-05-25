<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AI Quant Researcher | Interactive Portfolio</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script type="text/javascript" id="MathJax-script" async
    src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
  </script>
</head>
<body class="bg-gray-950 text-white font-sans">

  <!-- Hero Section -->
  <section class="text-center py-20 px-4">
    <h1 class="text-5xl font-bold text-blue-400 mb-4">AI / Quant Researcher</h1>
    <p class="text-xl text-gray-300 max-w-2xl mx-auto">Exploring the synergy between stochastic calculus and generative AI for advanced video generation models.</p>
  </section>

  <!-- Tool Icons -->
  <section class="py-10 px-4">
    <h2 class="text-3xl text-center mb-6 font-semibold text-purple-400">🛠️ Core Tools</h2>
    <div class="grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
      <div class="bg-gray-800 p-6 rounded-xl hover:scale-105 transition-transform">
        <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" class="w-12 h-12 mx-auto mb-2" />
        <p>TensorFlow</p>
      </div>
      <div class="bg-gray-800 p-6 rounded-xl hover:scale-105 transition-transform">
        <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" class="w-12 h-12 mx-auto mb-2" />
        <p>PyTorch</p>
      </div>
      <div class="bg-gray-800 p-6 rounded-xl hover:scale-105 transition-transform">
        <img src="https://www.vectorlogo.zone/logos/numpy/numpy-icon.svg" class="w-12 h-12 mx-auto mb-2" />
        <p>NumPy</p>
      </div>
      <div class="bg-gray-800 p-6 rounded-xl hover:scale-105 transition-transform">
        <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" class="w-12 h-12 mx-auto mb-2" />
        <p>OpenCV</p>
      </div>
    </div>
  </section>

  <!-- Black-Scholes Formula -->
  <section class="py-16 px-6 bg-gray-900 mt-10">
    <h2 class="text-3xl mb-4 text-cyan-300">📈 Black-Scholes Equation</h2>
    <p class="mb-4 text-gray-300">Used in option pricing, this PDE forms the base for stochastic modelling:</p>
    <div class="bg-gray-800 p-6 rounded-xl overflow-auto">
      <p class="text-lg text-white">
        $$\frac{\partial V}{\partial t} + \frac{1}{2} \sigma^2 S^2 \frac{\partial^2 V}{\partial S^2} + rS \frac{\partial V}{\partial S} - rV = 0$$
      </p>
    </div>
  </section>

  <!-- Stochastic Calculus Explanation -->
  <section class="py-16 px-6">
    <h2 class="text-3xl mb-4 text-emerald-300">📚 Stochastic Calculus in Generative AI</h2>
    <p class="text-gray-300 mb-6 max-w-3xl">
      Stochastic differential equations (SDEs), particularly Itô calculus, help model noise, randomness, and dynamic evolution in AI systems.
      In video generation models (e.g., diffusion models), the reverse-time SDE is learned to generate realistic frames from noise.
    </p>
    <div class="bg-gray-800 p-6 rounded-xl">
      <p class="text-lg">
        $$dX_t = \mu(X_t, t)dt + \sigma(X_t, t)dW_t$$
      </p>
    </div>
  </section>

  <!-- Video Generation Model -->
  <section class="py-16 px-6 bg-gray-900">
    <h2 class="text-3xl mb-4 text-pink-400">🎥 AI Video Generation Model</h2>
    <p class="text-gray-300 mb-6 max-w-3xl">
      Our generative pipeline leverages stochastic sampling and variational methods for producing temporally consistent and semantically rich video. Tools like Latent Diffusion, GANs, and Transformers are combined.
    </p>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="bg-gray-800 p-6 rounded-xl">
        <h3 class="text-xl text-white mb-2">Model Pipeline</h3>
        <ul class="list-disc list-inside text-gray-300">
          <li>Text-to-Latent Embedding (CLIP/BERT)</li>
          <li>Stochastic Video Diffusion (Reverse SDE)</li>
          <li>Temporal Consistency Filter</li>
          <li>Neural Rendering</li>
        </ul>
      </div>
      <div class="bg-gray-800 p-6 rounded-xl">
        <h3 class="text-xl text-white mb-2">Equations in Play</h3>
        <p>
          $$ \nabla_{\theta} \mathbb{E}_{q(x_t|x_0)}[\log p_\theta(x_{t-1}|x_t)] $$
        </p>
        <p class="text-gray-400 text-sm mt-2">Gradient of ELBO for denoising steps in diffusion models.</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="py-10 text-center text-gray-500">
    Made with ❤️ by a Quant-AI Researcher | <a href="#" class="underline hover:text-white">GitHub</a>
  </footer>

</body>
</html>
