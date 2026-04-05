<div align="center">
  <h1><a href="https://viratiakiranandhanreddy.github.io/animated-silk-background-three-js/">animated-silk-background-three-js</a></h1>
  <p><em>A beautiful animated silk texture background effect created with Three.js and custom GLSL shaders.</em></p>
</div>

<br>

## Overview

This project creates a smooth, flowing silk-like animation that fills the entire viewport. The effect is generated entirely through shader-based rendering, providing excellent performance even on lower-end devices.

## Features

- **Shader-Based Animation**: Custom vertex and fragment shaders create a procedural silk texture effect
- **Dynamic Patterns**: Combines sine waves and noise functions for organic, fluid motion
- **Customizable Parameters**:
  - `uColor`: Background color (default: purple `#8604f8`)
  - `uSpeed`: Animation speed multiplier
  - `uScale`: Pattern scale
  - `uRotation`: UV rotation angle
  - `uNoiseIntensity`: Noise distortion strength
- **Responsive Design**: Automatically adjusts to window resizing
- **High Performance**: Optimized rendering with pixel ratio handling

## Usage

Simply open `index.html` in a modern web browser. The animation will begin automatically.

### Customization

You can modify the uniform values in `three.js` to change the appearance:

```javascript
const uniforms = {
  uTime: { value: 0 },
  uSpeed: { value: 0.5 },        // Increase for faster animation
  uScale: { value: 1.0 },        // Increase for larger patterns
  uRotation: { value: 0.0 },     // Rotate the pattern
  uNoiseIntensity: { value: 1.5 }, // Increase for more texture
  uColor: { value: new THREE.Color('#8604f8') } // Change color
};
```

## Technical Details

### Shaders

**Vertex Shader**: Passes UV coordinates to the fragment shader for texture mapping.

**Fragment Shader**: 
- Implements a custom noise function for randomization
- Applies UV rotation and scaling
- Generates wave patterns using sine functions
- Combines multiple frequency layers for visual complexity

### Scene Setup

- Uses an orthographic camera for 2D rendering
- Creates a simple plane geometry that covers the entire viewport
- Implements WebGL rendering with antialiasing enabled

## Requirements

- Modern web browser with WebGL support
- Internet connection (loads Three.js from CDN)

## Browser Support

Works on all modern browsers that support:
- WebGL
- ES6 modules
- Three.js r160
