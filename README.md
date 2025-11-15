# 💡 Realistic Bulb for Three.js & WebXR

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Ultra-realistic 3D light bulb component with custom GLSL shader.  
**WebXR ready** - Optimized for Meta Quest 2/3.

---

## 🎬 Demos

| Demo | Description | Link |
|------|-------------|------|
| **Interactive Simulator** | Full-featured lighting simulator | [Try it](https://wory-bonbon.github.io/threejs-realistic-bulb/) |
| **Pier Demo** | Atmospheric pier lighting scene | [Try it](https://wory-bonbon.github.io/threejs-realistic-bulb/pier-demo.html) |
| **WebXR Version** | Quest/PC compatible standalone | [Try it](https://wory-bonbon.github.io/threejs-realistic-bulb/webxr-bulb.html) |
| **Minimal Example** | Shader-only, clean code | [Try it](https://wory-bonbon.github.io/threejs-realistic-bulb/shader-bulb.html) |

---

### 🎥 Demo Videos

**Pier Demo - Atmospheric Lighting**

[![Pier Demo](https://img.youtube.com/vi/3iOC1D9A5s8/maxresdefault.jpg)](https://youtu.be/3iOC1D9A5s8)

**Minimal Example - High-Quality Bulb**

[![Minimal Example](https://img.youtube.com/vi/lk4QX8G0RgE/maxresdefault.jpg)](https://youtu.be/lk4QX8G0RgE)

---

## 🎯 For Metaverse & Web3D Developers

- **Copy & paste ready** - Single function, no dependencies
- **VR optimized** - Auto quality switching for Quest
- **Customizable** - Color, intensity, multiple bulbs support
- **MIT License** - Use anywhere, even commercial projects

---

## 🚀 Quick Start

### Basic Usage
```javascript
// 1. Copy createHighQualityBulb() function from shader-bulb.html
// 2. Add to your scene
const bulb = createHighQualityBulb(0, 3, 0);
scene.add(bulb.group);
bulb.pointLight.intensity = 22;
bulb.pointLight.color.setHex(0xffaa33);
```

### WebXR Usage
See `webxr-bulb.html` for Meta Quest optimization

---

## ✨ Technical Features

### Custom GLSL Shader
- Fresnel effect (edge glow)
- Distance-based light falloff
- Height gradient illumination
- Realistic glass refraction (IOR 1.52)
- Flickering animation

### Geometry
- 220-point Bézier curve bulb shape
- 240-segment LatheGeometry
- Spiral tungsten filament (TubeGeometry)
- Accurate E26 socket model

### Performance
- **High Quality Mode**: Full shader effects (~60fps on desktop)
- **Low Quality Mode**: Quest-optimized (~72fps on Quest 2)
- Auto device detection

### Default Bulb Scale
The high-quality bulb uses realistic proportions:
- **Total height**: ~4.1 units (3.2 glass + 0.9 socket)
- **Base scale**: 1.0 (original size)
- **Recommended range**: 0.2-0.8 for compact scenes
- **Pier demo example**: 0.2 scale at Y=0.4 (ground level)

Adjust via `group.scale.set(x, y, z)` to fit your scene.

---

## 🛠️ Use Cases

- Metaverse lighting fixtures
- VR interior design apps
- Architectural visualization
- Web3D showcases
- Three.js learning projects

---

## 📦 What's Included
```
threejs-realistic-bulb/
├── index.html              # Interactive simulator (try all features)
├── pier-demo.html          # Atmospheric pier scene (NEW)
├── webxr-bulb.html         # WebXR standalone (Quest ready)
├── shader-bulb.html        # Minimal example (copy from here)
├── README.md
└── LICENSE (MIT)
```

---

## 📄 License

MIT License - Use freely in personal/commercial projects