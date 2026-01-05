# 4D Static Universe Slicer

A browser-based research tool for visualizing 4D geometric shapes by slicing them into 3D cross-sections.

[**Launch Live Visualizer**](https://static-universe-slicer.vercel.app/)

## 🌌 Time is Not Fundamental

Modern theoretical physics—from the **Amplituhedron** to the **Cosmological Polytope**—points to a radical conclusion: **Spacetime is not fundamental.** The universe is likely a static, high-dimensional geometric object, and what we perceive as "Time Evolution" or "Motion" is merely the result of taking a 3D slice through this static 4D structure.

This tool is built to let you explore that concept intuitively.

## Key Features

*   **Inequality Slicer**: Unlike standard mesh visualizers, this engine renders shapes defined by **Linear Inequalities** ($ax + by + cz + dw \le e$). This allows for the visualization of "Positive Geometries" often used in theoretical physics.
*   **Wavefunction Monitor**: A dual-axis graph that monitors the **Topology** (Vertex Count - Cyan) and **Amplitude** (Volume - Violet) simultaneously. Provides insight into the relationship between discrete geometric phases and continuous physical probability.
*   **OEIS Extractor**: Analyzes the "Topological Sequence" of the current shape (e.g., `4, 6, 8, 4`) and generates a direct search link to the **On-Line Encyclopedia of Integer Sequences**, connecting 4D geometry to Number Theory.
*   **Universe Hunter**: A generative engine that searches the multiverse for "Rare" polytopes. It uses drift-based asymmetry and a topology scoring algorithm to find universes with complex, multi-peak phase transitions.
*   **Interactive Presets**: Includes pre-calculated inequality sets for:
    *   **Complex Crystal** (A high-symmetry 24-Cell variant)
    *   **Resonance Experiment** (A "Needle" universe simulating physical scattering thresholds)
    *   **Hypercube** (Tesseract)
    *   **16-Cell** (Cross Polytope)
    *   **Duocylinder** (Cyclic approximation)
    *   **Simplex** (5-Cell)
*   **Zero-Build Architecture**: Written in Vanilla JS + Three.js. No build steps, webpack, or complex dependencies required.

## How to Use

1.  **Select a Preset**: Use the left sidebar to load different 4D shapes.
2.  **Hunt for Universe**: Click the **"HUNT FOR UNIVERSE"** button. The engine will scan dozens of random candidates and select the one with the most interesting topological features (multi-peak graphs).
3.  **Slice Time ($W$)**: Drag the main slider to move the 3D slicing plane through the 4th dimension.
3.  **Analyze Wavefunction**: Watch the bottom graph. 
    *   **Cyan Line (Topology)**: Step-wise graph of vertex count. Sharp jumps indicate Singularities.
    *   **Violet Line (Amplitude)**: Smooth curve of Volume/Probability.
    *   **Hover**: Hover over the graph for precise Floating Point data.
4.  **Combinatorics**: Click **"GENERATE SEQUENCE"** to extract the topological phases and instantly search them in the OEIS database.
5.  **Custom Data**: You can paste your own JSON array of inequalities into the "Inequality Matrix" text area.
    *   Format: `[[a, b, c, d, e], ...]`
    *   Represents: $ax + by + cz + dw \le e$

## Project Structure

*   `index.html`: Contains the entire application (UI, Math Engine, Rendering).
*   `assets`: (Optional) Static assets for social previews.

## Contributing

This project is built to be extremely accessible. To modify or run it locally:

1.  Clone the repository.
2.  Open `index.html` in any web browser.
3.  That's it.

**Math & Logic:**
The core vertex enumeration logic is located within the `<script>` tag in `index.html`. It solves for the intersection of plane triplets to generate the convex hull of the 3D cross-section.
