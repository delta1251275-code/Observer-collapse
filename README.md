# Δ = THE OBSERVER

Welcome to **Δ = THE OBSERVER**, an interactive Bell-state CHSH simulation in a noisy cavity! This project brings quantum entanglement and wavefunction collapse to life, running directly in your browser using QuTiP and Pyodide.

## Live Demo
Experience the simulation live:  
[**https://deviousdust-del.github.io/Observer-Collapse/**](https://deviousdust-del.github.io/Observer-Collapse/)

- Click "Collapse Now" to collapse the wavefunction and see the CHSH value (S), noise impact, and thematic output.
- Note: Best viewed on a desktop browser (e.g., Chrome, Firefox) due to mobile compatibility limitations with Pyodide.

## Features
- Real-time simulation of a Bell-state CHSH inequality test.
- Noisy cavity environment with parameters like noise level (0.05) and 5000 trials.
- Dynamic progress bar and stylized results (e.g., pulsing "SPOOKY LINK SURVIVED" text).

## How It Works
The simulation models two entangled qubits coupled to noisy cavities, evolving via the master equation (QuTiP). It calculates the CHSH parameter (S) to test quantum non-locality:
- Ideal quantum max: ~2.828 (violates Bell's inequality).
- Classical limit: ≤2.
- Noise reduces S, as seen in the output (e.g., S = -0.4923 with 117.4% noise loss in a sample run).

## Tech Stack
- **HTML/CSS/JavaScript**: Structures the page and handles interactivity.
- **Pyodide**: Executes Python in the browser.
- **QuTiP**: Quantum toolbox for Python, powering the simulation.
- **NumPy**: Supports numerical computations.

## Getting Started
1. Visit the [live demo](#live-demo) to run the simulation.
2. For local testing, clone this repo, open `index.html` in a modern browser, and ensure an internet connection for Pyodide.
3. Adjust parameters (e.g., `extra_noise` in the Python code) by editing `index.html` and committing changes.

## Known Issues
- Mobile browsers may stall at "Loading Python…" due to WebAssembly support—use a desktop for now.
- Report bugs or suggest enhancements via the [Issues tab](https://github.com/deviousduu/Observer-Collapse/issues).

## Author
Created by [deviousdust-del](https://github.com/deviousduu).

## License
[Optional: Add a license, e.g., MIT. You can generate one via the "Add file" dropdown later if desired.]
