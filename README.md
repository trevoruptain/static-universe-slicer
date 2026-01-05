# The Static Universe Slicer

> *"We are building the visualization layer for the post-spacetime era of physics."*

## 🌌 Mission Statement: Time is Not Fundamental

Modern theoretical physics—from the **Amplituhedron** to the **Cosmological Polytope**—points to a radical conclusion: **Spacetime is not fundamental.** The universe is likely a static, high-dimensional geometric object, and what we perceive as "Time Evolution" or "Motion" is merely the result of taking a 3D slice through this static 4D structure.

**The Static Universe Slicer** is built on this intuition. We are not simulating objects moving through time; we are exploring the geometry of valid particle interactions frozen in a higher dimension. By enabling researchers to intuitively slice through these shapes, we hope to uncover the hidden combinatorial patterns that govern our reality.

## 🔭 The Current MVP

This tool is a lightweight, browser-based visualizer designed to bridge the gap between abstract algebra and geometric intuition.

### Key Logic: The Inequality Slicer
Unlike standard 3D engines that rely on vertex lists, our core engine works with **Linear Inequalities (Half-Spaces)**. This is crucial because high-level physics data usually comes in the form of kinematic constraints (e.g., $s_{ij} > 0$), not pre-calculated vertices.

*   **Input**: JSON array of 4D plane equations ($ax + by + cz + dw \le e$).
*   **The "Time" Slider**: Controls the $W$-axis. As you drag the slider, the engine dynamically substitutes $W$, reduces the system to 3D constraints, solves for the vertices via linear algebra, and generates the mesh.
*   **Presets**:
    *   **Complex Crystal**: A variant of the 24-Cell, demonstrating complex face transitions.
    *   **Simplex**: The "hello world" of positive geometry, related to the Amplituhedron.

### Technical Stack
*   **Engine**: Three.js (WebGL) for rendering.
*   **Algorithm**: Dynamic Vertex Enumeration & Convex Hull generation.
*   **Architecture**: Vanilla JavaScript (ES Modules). No build steps, no webpack, no bloat. Pure math and graphics.

---

## 🚀 The Future Roadmap: Why We Are Here

We are transforming this from a visualization toy into a research-grade tool for Quantum Gravity and Amplitudeology.

### 1. Singularity Detection (The Physics of Zero Volume)
In scattering amplitudes, "singularities" (where the volume of the shape pinches to zero) correspond to physical particles becoming real or poles in a Feynman integral.
*   **Goal**: Automatically flag the slider values ($W$) where faces collide or volume vanishes.

### 2. Kinematic Flow Integration
We plan to bypass manual JSON entry.
*   **Goal**: Integrate graph-theory algorithms to generate inequality sets directly from **Feynman diagrams** or Planar Graphs. You draw the interaction; we generate the Positive Geometry.

### 3. The OEIS Scraper
Geometry often encodes number theory.
*   **Goal**: Automatically count the faces ($f$-vector) of the sliced shape at every step and query the [Online Encyclopedia of Integer Sequences](https://oeis.org/) to find hidden combinatorial patterns in the data.

### 4. N-Dimensional Support
Supergravity theories often live in 10 or 11 dimensions.
*   **Goal**: Generalize the slicer to handle $N > 4$, allowing for "double slicing" or multi-axis projection.

---

## 🛠️ Getting Started

### Installation
There is no installation. The universe is static, and so is this code.
1.  Clone the repo.
2.  Open `index.html` in any browser.
3.  Slice.

### Contributing
We welcome both **Software Engineers** who love geometry and **Physicists** who code.
- **Engineers**: Help us optimize the Vertex Enumeration algorithm for $N>100$ planes.
- **Physicists**: Submit new JSON presets for interesting polytopes (Associahedra, Permutahedra).

Join us in decoding the geometry of the universe.
