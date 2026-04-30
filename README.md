# Algorithm Visualizer Suite

This repository contains a collection of four interactive algorithm visualizers built for the BSD 404 (Algorithm Analysis) final project. Each visualizer is a standalone, self-contained HTML file built with pure vanilla HTML, CSS, and JavaScript, with **zero external dependencies**.

- **Student:** Arham bin Azad (20220001121)
- **Course:** BSD 404 Algorithm Analysis
- **Instructor:** Dr. Arash Kermani

## Project Overview

The goal of this project is to provide clear, interactive, and educational demonstrations of several key algorithms, making it easier for students to understand complex topics in a visual and intuitive way. The primary constraint was to avoid all external libraries and build systems, meaning each visualizer is a single file that can be opened directly in any modern web browser.

## Running the Project

No installation or build process is required.

1.  Clone the repository.
2.  Open any of the `.html` files directly in your web browser.

Alternatively, you can serve the files locally using a simple Python web server:

```bash
# From the project's root directory:
python -m http.server 8000
```

Then, navigate to `http://localhost:8000` in your browser and click on the visualizer you'd like to use.

## Included Visualizers

| File | Algorithm |
|------|-----------|
| `fft-polynomial.html` | FFT Polynomial Multiplication |
| `miller-rabin.html` | Miller-Rabin Primality Testing |
| `rabin-karp.html` | Rabin-Karp String Matching |
| `metric-tsp.html` | 2-Approximation for Metric TSP |

## Features

All visualizers share a common set of features and a consistent layout for ease of use:

- **Playback Controls:** Play, pause, step forward, and reset the animation.
- **Speed Slider:** Adjust the animation speed from 0.25× to 4×.
- **Interactive History:** A history table logs every step of the algorithm. Clicking a row instantly jumps the visualization to that state.
- **Pseudocode Highlighting:** The line of pseudocode corresponding to the current animation step is highlighted.
- **Detailed Tooltips:** Hover over any line of pseudocode for a detailed explanation of that step.
- **Live Counters:** Key operations are counted in real-time as the algorithm runs.
- **Educational Notes:** Each tool includes collapsible lecture notes explaining the theory, complexity, and key concepts behind the algorithm.
- **Responsive Design:** The layout adjusts for smaller screens, making it usable on mobile devices.

## Architecture

The visualizers are built on a simple but effective pattern:

- **Pre-computed Steps:** Before the animation begins, the entire sequence of algorithmic steps is computed and stored in an array. This allows for instant seeking (jumping to any step), smooth playback, and decoupling of the algorithm's logic from the animation's timing.
- **Self-Contained Files:** All necessary HTML, CSS, and JavaScript are contained within a single `.html` file for each visualizer. This ensures maximum portability and simplicity.
- **Inline SVG for Visualization:** Animations are rendered using inline SVG, which allows for easy labeling and interaction with individual components of the visualization.
- **CSS Variables for Theming:** A dark theme is used across all tools, with a unique accent color for each algorithm to make them visually distinct.

