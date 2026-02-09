<div align="center">
  <h1><a href="https://viratiakiranandhanreddy.github.io/animated-silk-background-three-js/">animated-silk-background-three-js</a></h1>
  <p><em>A beautiful animated silk texture background effect created with Three.js and custom GLSL shaders.</em></p>
</div>

<br>

## Overview

This project creates a smooth, flowing silk-like animation that fills the entire viewport. The effect is generated entirely through shader-based rendering, providing excellent performance even on lower-end devices.

---

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

---

## Usage

Simply open `index.html` in a modern web browser. The animation will begin automatically.

---

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

---

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

---

## Requirements

- Modern web browser with WebGL support
- Internet connection (loads Three.js from CDN)

---

## Browser Support

Works on all modern browsers that support:
- WebGL
- ES6 modules
- Three.js r160

---

## **🤝 Contributing**

Pull requests are welcome!

To contribute:

1. Fork the repository
2. Create a new branch
3. Add your changes
4. Open a PR

---

## ⭐ Support
<kbd>If you like this project, consider giving it a star ⭐ on GitHub — it helps a lot.</kbd>

---

## 🌐 Social & Links

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/viratiakiranandhanreddy/)
[![X](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Viratiaki53)
[![Instagram](https://img.shields.io/badge/Instagram-E1306C?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/viratiaki53)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/ViratiAkiraNandhanReddy)
[![Gist](https://img.shields.io/badge/Gist-2b3137?style=for-the-badge&logo=github&logoColor=white)](https://gist.github.com/ViratiAkiraNandhanReddy)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@ViratiAkiraNandhanReddy)
[![Website](https://img.shields.io/badge/Website-0077b6?style=for-the-badge&logoColor=white)](https://viratiakiranandhanreddy.github.io/CaesarCipher.extended/)
[![Mail](https://img.shields.io/badge/Mail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:contact.viratiakiranandhanreddy+github@gmail.com)

---

## 📝 License

<p align="center"><kbd>&copy; 2025 <a href="https://github.com/ViratiAkiraNandhanReddy">ViratiAkiraNandhanReddy</a>. This project is licensed under the <i>MIT License</i>.</kbd></p>

---

## 👤 Author

### Developed by [ViratiAkiraNandhanReddy](https://github.com/ViratiAkiraNandhanReddy)

> 💤 - PASSIVE MAINTENANCE : Mean the project is no longer actively developed ***( NO New Features And Regular Updates )***, but the maintainer will respond only when an issue or PR is raised. Feel free to fork and continue development!

---

<h3 align="center"> 🌟 Questions, suggestions, or want to contribute? Open an issue or pull request on GitHub! 🌟 </h3>

<p align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=0e8fff&height=100&section=footer" width="100%" /> </p>
