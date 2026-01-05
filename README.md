# 4D Static Universe Slicer

A browser-based research tool for visualizing 4D geometric shapes by slicing them into 3D cross-sections.

[**Launch Live Visualizer**](https://static-universe-slicer.vercel.app/)

## 🌌 Time is Not Fundamental

Modern theoretical physics—from the **Amplituhedron** to the **Cosmological Polytope**—points to a radical conclusion: **Spacetime is not fundamental.** The universe is likely a static, high-dimensional geometric object, and what we perceive as "Time Evolution" or "Motion" is merely the result of taking a 3D slice through this static 4D structure.

This tool is built to let you explore that concept intuitively.

## Key Features

*   **Inequality Slicer**: Unlike standard mesh visualizers, this engine renders shapes defined by **Linear Inequalities** ($ax + by + cz + dw \le e$). This allows for the visualization of "Positive Geometries" often used in theoretical physics.
*   **Singularity Scanner**: A real-time topology graph that plots the Vertex Count against the 4th dimension ($W$). This helps identify "Phase Transitions" or singularities where the geometry drastically changes.
*   **Interactive Presets**: Includes pre-calculated inequality sets for:
    *   **Complex Crystal** (24-Cell variant)
    *   **Hypercube** (Tesseract)
    *   **16-Cell** (Cross Polytope)
    *   **Duocylinder** (Approximation)
    *   **Simplex** (5-Cell)
*   **Zero-Build Architecture**: Written in Vanilla JS + Three.js. No build steps, webpack, or complex dependencies required.

## How to Use

1.  **Select a Preset**: Use the left sidebar to load different 4D shapes.
2.  **Slice Time ($W$)**: Drag the main slider to move the 3D slicing plane through the 4th dimension.
3.  **Analyze Topology**: Watch the bottom graph. The blue line represents the complexity (number of vertices) of the current slice.
    *   **Jump**: Click anywhere on the graph to instantly view the shape at that specific $W$ coordinate.
4.  **Custom Data**: You can paste your own JSON array of inequalities into the "Inequality Matrix" text area.
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
