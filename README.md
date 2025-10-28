<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Δ = THE OBSERVER</title>
  <style>
    body {
      font-family: 'Courier New', monospace;
      background: #0a0a0a;
      color: #0f0;
      margin: 0;
      padding: 20px;
      line-height: 1.6;
    }
    h1, h2, h3 { color: #0f0; text-shadow: 0 0 5px #0f0; }
    a { color: #0ff; text-decoration: none; }
    a:hover { text-decoration: underline; }
    pre { background: #111; padding: 15px; border: 1px solid #0f0; overflow-x: auto; }
    .container { max-width: 900px; margin: auto; }
    .pulse { animation: pulse 1.5s infinite; }
    @keyframes pulse { 0% { opacity: 1; } 50% { opacity: 0.5; } 100% { opacity: 1; } }
  </style>
</head>
<body>
<div class="container">

<h1>Δ = THE OBSERVER</h1>

<p>Welcome to <strong>Δ = THE OBSERVER</strong>, an interactive Bell-state CHSH simulation in a noisy cavity! This project brings quantum entanglement and wavefunction collapse to life, running directly in your browser using QuTiP and Pyodide.</p>

<h2>Live Demo</h2>
<p>Experience the simulation live:<br>
<strong><a href="https://delta1251275-code.github.io/Observer-collapse/" target="_blank">https://delta1251275-code.github.io/Observer-collapse/</a></strong></p>

<ul>
  <li>Click "Collapse Now" to collapse the wavefunction and see the CHSH value (S), noise impact, and thematic output.</li>
  <li><strong>Note:</strong> Best viewed on a desktop browser (e.g., Chrome, Firefox) due to mobile compatibility limitations with Pyodide.</li>
</ul>

<h2>Features</h2>
<ul>
  <li>Real-time simulation of a Bell-state CHSH inequality test.</li>
  <li>Noisy cavity environment with parameters like noise level (0.05) and 5000 trials.</li>
  <li>Dynamic progress bar and stylized results (e.g., pulsing "SPOOKY LINK SURVIVED" text).</li>
</ul>

<h2>How It Works</h2>
<p>The simulation models two entangled qubits coupled to noisy cavities, evolving via the master equation (QuTiP). It calculates the CHSH parameter (S) to test quantum non-locality:</p>
<ul>
  <li><strong>Ideal quantum max:</strong> ~2.828 (violates Bell's inequality).</li>
  <li><strong>Classical limit:</strong> ≤2.</li>
  <li><strong>Noise reduces S</strong>, as seen in the output (e.g., S = -0.4923 with 117.4% noise loss in a sample run).</li>
</ul>

<h2>Tech Stack</h2>
<ul>
  <li><strong>HTML/CSS/JavaScript</strong>: Structures the page and handles interactivity.</li>
  <li><strong>Pyodide</strong>: Executes Python in the browser.</li>
  <li><strong>QuTiP</strong>: Quantum toolbox for Python, powering the simulation.</li>
  <li><strong>NumPy</strong>: Supports numerical computations.</li>
</ul>

<h2>Getting Started</h2>
<ol>
  <li>Visit the <a href="#live-demo">live demo</a> to run the simulation.</li>
  <li>For local testing, clone this repo, open <code>index.html</code> in a modern browser, and ensure an internet connection for Pyodide.</li>
  <li>Adjust parameters (e.g., <code>extra_noise</code> in the Python code) by editing <code>index.html</code> and committing changes.</li>
</ol>

<h2>Known Issues</h2>
<ul>
  <li>Mobile browsers may stall at "Loading Python…" due to WebAssembly support—use a desktop for now.</li>
  <li>Report bugs or suggest enhancements via the <a href="https://github.com/delta1251275-code/Observer-collapse/issues" target="_blank">Issues tab</a>.</li>
</ul>

<h2>Author</h2>
<p>Created by <a href="https://github.com/delta1251275-code" target="_blank">delta1251275-code</a>.</p>

<h2>License</h2>
<p><a href="LICENSE">MIT License</a> — Free to use, modify, and distribute.</p>

<hr>
<p style="text-align:center; font-size:0.9em;">
  <span class="pulse">SPOOKY ACTION AT A DISTANCE — STILL ALIVE</span>
</p>

</div>
</body>
</html>
