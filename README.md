# 🎨 3D Superformula Generator

An interactive web application for generating and exploring 3D shapes using the Gielis Superformula. Create mesmerizing mathematical forms with real-time parameter adjustment and 3D visualization.

![Superformula Demo](https://img.shields.io/badge/Three.js-r128-blue) ![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- **Interactive 3D Visualization**: Pan, tilt, and zoom with intuitive mouse controls
- **Real-time Parameter Adjustment**: 12 sliders for complete control over the superformula
- **Random Shape Generator**: Discover interesting forms with a single click
- **Responsive Design**: Works seamlessly on desktop and mobile browsers
- **Self-Contained**: Single HTML file with all dependencies loaded from CDN

## 🚀 Quick Start

1. Clone this repository:
```bash
git clone https://github.com/yourusername/3d-superformula.git
cd 3d-superformula
```

2. Open `index.html` in your web browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

That's it! No build process or dependencies to install.

## 🎮 Controls

### Mouse Controls
- **Left Click + Drag**: Rotate the view
- **Right Click + Drag**: Pan the camera
- **Scroll Wheel**: Zoom in/out

### Interface
- **🎲 Generate Random Shape**: Creates a random combination of parameters
- **↺ Reset to Default**: Returns all parameters to their default values
- **Sliders**: Adjust individual parameters in real-time

## 📐 The Superformula

The superformula, created by Johan Gielis, is a generalization of the superellipse that can describe a wide variety of natural and abstract shapes. The formula is:

```
r(φ) = (|cos(m·φ/4)/a|^n2 + |sin(m·φ/4)/b|^n3)^(-1/n1)
```

For 3D shapes, we apply this formula to both latitude (φ) and longitude (θ) angles.

### Parameters

**Latitude Parameters (φ)**
- `m₁`: Number of symmetries (0-20)
- `n1₁`, `n2₁`, `n3₁`: Shape exponents (0.1-10)
- `a₁`, `b₁`: Scaling factors (0.1-3)

**Longitude Parameters (θ)**
- `m₂`: Number of symmetries (0-20)
- `n1₂`, `n2₂`, `n3₂`: Shape exponents (0.1-10)
- `a₂`, `b₂`: Scaling factors (0.1-3)

**Mesh Settings**
- `Resolution`: Mesh detail level (16-128)

## 🎯 Interesting Combinations

Try these parameter sets for beautiful shapes:

### Star Shape
- m₁ = 5, n1₁ = 2, n2₁ = 7, n3₁ = 7
- m₂ = 5, n1₂ = 2, n2₂ = 7, n3₂ = 7

### Flower
- m₁ = 8, n1₁ = 1, n2₁ = 4, n3₁ = 8
- m₂ = 8, n1₂ = 1, n2₂ = 4, n3₂ = 8

### Crystal
- m₁ = 6, n1₁ = 0.5, n2₁ = 1.7, n3₁ = 1.7
- m₂ = 6, n1₂ = 0.5, n2₂ = 1.7, n3₂ = 1.7

### Seashell
- m₁ = 3, n1₁ = 4.5, n2₁ = 10, n3₁ = 10
- m₂ = 4, n1₂ = 2, n2₂ = 2, n3₂ = 2

## 🛠️ Technical Details

### Built With
- **Three.js r128**: 3D graphics library
- **Vanilla JavaScript**: No frameworks required
- **HTML5 & CSS3**: Modern web standards

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

### Performance
- Optimized vertex generation
- Efficient mesh updates
- Smooth 60fps rendering on modern hardware

## 📁 Project Structure

```
3d-superformula/
├── index.html          # Main application file
├── README.md           # This file
└── LICENSE            # MIT License
```

## 🤝 Contributing

Contributions are welcome! Here are some ideas for enhancements:

- Export shapes as OBJ/STL files
- Add texture mapping options
- Implement animation presets
- Add color scheme customization
- Create a gallery of saved shapes

To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📚 Resources

- [Superformula on Wikipedia](https://en.wikipedia.org/wiki/Superformula)
- [Three.js Documentation](https://threejs.org/docs/)
- [Johan Gielis's Research](http://www.genicap.com/)

## 🙏 Acknowledgments

- Johan Gielis for the superformula
- Three.js team for the amazing 3D library
- The mathematical visualization community

---

Made with ❤️ and mathematics
