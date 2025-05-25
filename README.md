<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AI × Quant Researcher</title>
  <link rel="stylesheet" href="style.css" />
  <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
  <script id="MathJax-script" async
    src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
  </script>
</head>
<body>
  <header>
    <h1>AI × Quant Researcher Portfolio</h1>
    <p>Static Showcase of Tools, Visuals, and Mathematical Foundations</p>
  </header>

  <section class="tools-section">
    <h2>🔧 AI Tools</h2>
    <div class="grid-container">
      <div><img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg"><p>TensorFlow</p></div>
      <div><img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg"><p>PyTorch</p></div>
      <div><img src="https://www.vectorlogo.zone/logos/numpy/numpy-icon.svg"><p>NumPy</p></div>
      <div><img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg"><p>OpenCV</p></div>
      <div><img src="https://www.vectorlogo.zone/logos/scikit_learn/scikit_learn-icon.svg"><p>scikit-learn</p></div>
      <div><img src="https://www.vectorlogo.zone/logos/kerasio/kerasio-icon.svg"><p>Keras</p></div>
    </div>

    <h2>💹 Quant & Finance Tools</h2>
    <div class="grid-container">
      <div><img src="https://upload.wikimedia.org/wikipedia/commons/8/8a/QuantLib_logo.svg"><p>QuantLib</p></div>
      <div><img src="https://upload.wikimedia.org/wikipedia/commons/8/86/Excel_2013_logo.svg"><p>Excel</p></div>
      <div><img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Matplotlib_logo.svg"><p>Matplotlib</p></div>
      <div><img src="https://upload.wikimedia.org/wikipedia/commons/1/10/Pandas_logo.svg"><p>Pandas</p></div>
    </div>
  </section>

  <section class="math-section">
    <h2>📐 Core Math in AI & Quant</h2>
    <ul>
      <li><strong>Linear Algebra:</strong> \( \mathbf{y} = \mathbf{W}\mathbf{x} + \mathbf{b} \)</li>
      <li><strong>Probability:</strong> \( P(x) = \frac{\text{favorable outcomes}}{\text{total outcomes}} \)</li>
      <li><strong>Bayes Theorem:</strong> \( P(A|B) = \frac{P(B|A) P(A)}{P(B)} \)</li>
      <li><strong>Gradient Descent:</strong> \( \theta = \theta - \alpha \nabla J(\theta) \)</li>
      <li><strong>Loss Function (MSE):</strong> \( L = \frac{1}{n} \sum_{i=1}^{n}(y_i - \hat{y}_i)^2 \)</li>
      <li><strong>Softmax:</strong> \( \sigma(z_i) = \frac{e^{z_i}}{\sum_j e^{z_j}} \)</li>
      <li><strong>Entropy:</strong> \( H(p) = - \sum_x p(x) \log p(x) \)</li>
      <li><strong>Black-Scholes PDE:</strong> 
        \( \frac{\partial V}{\partial t} + \frac{1}{2} \sigma^2 S^2 \frac{\partial^2 V}{\partial S^2} + rS \frac{\partial V}{\partial S} - rV = 0 \)
      </li>
      <li><strong>Itô Process:</strong> \( dX_t = \mu dt + \sigma dW_t \)</li>
      <li><strong>ELBO in Variational Inference:</strong> 
        \( \mathbb{E}_{q(z)}[\log p(x|z)] - D_{KL}(q(z)||p(z)) \)</li>
    </ul>
  </section>

  <footer>
    <p>© 2025 AI × Quant Static Portfolio | No JS frameworks used.</p>
  </footer>
</body>
</html>
