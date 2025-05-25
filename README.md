body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0d1117;
  color: #c9d1d9;
}

header {
  background: #161b22;
  text-align: center;
  padding: 2rem;
  color: #58a6ff;
}

header h1 {
  margin: 0;
  font-size: 2.5rem;
}

.section {
  padding: 2rem;
}

h2 {
  color: #79c0ff;
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  gap: 1rem;
}

.card {
  background: #1f2937;
  padding: 1rem;
  text-align: center;
  border-radius: 10px;
  transition: transform 0.3s;
}

.card:hover {
  transform: scale(1.05);
}

.card img {
  height: 50px;
  margin-bottom: 0.5rem;
  max-width: 100%;
}

ul {
  padding-left: 1.2rem;
  list-style-type: square;
}

li {
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

footer {
  text-align: center;
  padding: 1.5rem;
  background: #161b22;
  color: #8b949e;
  font-size: 0.9rem;
}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI × Quant Researcher</title>
  <link rel="stylesheet" href="style.css">
  <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
  <script id="MathJax-script" async 
    src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
  </script>
</head>
<body>
  <header>
    <h1>AI × Quant Researcher</h1>
    <p>All Mathematics & Tools Visualized — Fully Static</p>
  </header>

  <section class="section">
    <h2>🔧 AI Tools</h2>
    <div class="grid">
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Tensorflow_logo.svg" alt="TensorFlow"><p>TensorFlow</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/9/96/Pytorch_logo.png" alt="PyTorch"><p>PyTorch</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg" alt="NumPy"><p>NumPy</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Scikit_learn_logo_small.svg" alt="sklearn"><p>scikit-learn</p></div>
    </div>
  </section>

  <section class="section">
    <h2>💹 Quant & Finance Tools</h2>
    <div class="grid">
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/8/86/Excel_2013_logo.svg" alt="Excel"><p>Excel</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/1/10/Pandas_logo.svg" alt="Pandas"><p>Pandas</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" alt="Matplotlib"><p>Matplotlib</p></div>
      <div class="card"><img src="https://upload.wikimedia.org/wikipedia/commons/f/fd/QuantLib.png" alt="QuantLib"><p>QuantLib</p></div>
    </div>
  </section>

  <section class="section math">
    <h2>📐 Mathematics Used in AI & Quant</h2>
    <ul>
      <li><strong>Linear Algebra:</strong> \( \mathbf{y} = \mathbf{W}\mathbf{x} + \mathbf{b} \)</li>
      <li><strong>Gradient Descent:</strong> \( \theta = \theta - \alpha \nabla J(\theta) \)</li>
      <li><strong>Softmax:</strong> \( \sigma(z_i) = \frac{e^{z_i}}{\sum_j e^{z_j}} \)</li>
      <li><strong>Loss Function (MSE):</strong> \( L = \frac{1}{n} \sum_{i=1}^{n}(y_i - \hat{y}_i)^2 \)</li>
      <li><strong>Bayes Theorem:</strong> \( P(A|B) = \frac{P(B|A) P(A)}{P(B)} \)</li>
      <li><strong>Entropy:</strong> \( H(p) = - \sum_x p(x) \log p(x) \)</li>
      <li><strong>Itô Process:</strong> \( dX_t = \mu dt + \sigma dW_t \)</li>
      <li><strong>Black-Scholes PDE:</strong> 
        \( \frac{\partial V}{\partial t} + \frac{1}{2} \sigma^2 S^2 \frac{\partial^2 V}{\partial S^2} + rS \frac{\partial V}{\partial S} - rV = 0 \)
      </li>
      <li><strong>ELBO in Diffusion Models:</strong> 
        \( \mathbb{E}_{q(z)}[\log p(x|z)] - D_{KL}(q(z)||p(z)) \)</li>
    </ul>
  </section>

  <footer>
    <p>© 2025 Static AI + Quant Portfolio • Hosted on GitHub Pages</p>
  </footer>
</body>
</html>

