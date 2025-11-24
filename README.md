# Shader Lesson Examples

This directory contains a series of interactive examples demonstrating the concepts from the "Shaders" article. Each example is a self-contained HTML file that you can open directly in your web browser.

Source: [Making Software - Shaders](https://www.makingsoftware.com/chapters/shaders)

## How to Run

Simply double-click any of the `.html` files to open them in your default browser. No server is required as they load Three.js from a CDN.

## Examples

### 1. [Solid Color Shader](01_solid_color.html)
**Concept:** The simplest fragment shader.
**What to look for:** A solid red square. This demonstrates the basic setup of a Three.js scene with a custom `ShaderMaterial`. The fragment shader returns a single color `vec4(1.0, 0.0, 0.0, 1.0)`.

### 2. [Horizontal Gradient](02_gradient_x.html)
**Concept:** Using UV coordinates.
**What to look for:** A gradient fading from black (left) to red (right). This introduces `varying` variables to pass the UV coordinates from the vertex shader to the fragment shader.

### 3. [Vertical Gradient](03_gradient_y.html)
**Concept:** Using different vector components.
**What to look for:** A gradient fading from black (bottom) to green (top). Similar to the previous example but uses the Y component of the UV coordinates.

### 4. [Animated Color](04_animated_color.html)
**Concept:** Uniforms and Time.
**What to look for:** A square that pulses between red and yellow/green. This introduces `uniforms`, which are variables passed from the CPU (JavaScript) to the GPU (Shader) that are constant for all pixels in a single frame but can change over time.

### 5. [Vertex Displacement](05_vertex_displacement.html)
**Concept:** Vertex Shaders.
**What to look for:** A wireframe plane with a moving sine wave. This demonstrates how the vertex shader can manipulate the position of vertices before they are drawn.

### 6. [Ripple Effect](06_ripple.html)
**Concept:** Advanced Vertex Manipulation.
**What to look for:** A complex ripple effect radiating from the center. This combines distance calculations with time-based animation in the vertex shader to create a dynamic 3D surface.
