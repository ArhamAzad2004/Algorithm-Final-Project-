# BSD 404 — Algorithm Visualizer

**Student:** Arham bin Azad (20220001121)
**Course:** BSD 404 — Algorithm Analysis
**Instructor:** Dr. Arash Kermani
**Deadline:** April 30, 2026

---

## Overview

Four interactive, step-by-step algorithm visualizers built as self-contained HTML files — no frameworks, no build tools, no internet required. Each tool lets you run preset examples or enter custom input, step through the algorithm at your own pace, and read inline lecture notes explaining the key concepts.

---

## Tools

| File | Algorithm | What it covers |
|------|-----------|----------------|
| [fft-polynomial.html](fft-polynomial.html) | FFT Polynomial Multiplication | Butterfly network, roots of unity, O(n log n) vs O(n²) |
| [miller-rabin.html](miller-rabin.html) | Miller-Rabin Primality Test | Square-and-multiply, Carmichael numbers, RSA key gen |
| [rabin-karp.html](rabin-karp.html) | Rabin-Karp String Matching | Rolling hash, spurious hits, expected O(\|P\|+\|T\|) |
| [metric-tsp.html](metric-tsp.html) | 2-Approximation for Metric TSP | MST lower bound, DFS walk, shortcutting, 2×OPT proof |

---

## How to Run

Open any `.html` file directly in a browser — no server needed.

The [index.html](index.html) navigation hub links all four tools from one page.

---

## Features (all four tools)

- Step-by-step animation with Play / Pause / Step / Reset controls
- Speed slider from 0.25× to 4×
- Clickable history table — click any past step to jump back to it
- Pseudocode panel with the current line highlighted and hover tooltips
- Live operation counters (comparisons, hash hits, butterfly ops, etc.)
- Collapsible lecture notes and worked examples
- Key Concept callout boxes for the core theoretical insight of each algorithm
- Fully responsive — single column below 980px

---

## Tech

Vanilla HTML + CSS + JavaScript. Zero external libraries or CDN calls. Each file is fully self-contained and opens offline.
