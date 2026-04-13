# Web Animation Game

An interactive web animation showcase featuring a character with dynamic animations, parallax scrolling backgrounds, and moving vehicles. Built with modern Web Animations API and CSS.

## 🚀 Live Demo

👉 [https://vasylpryimakdev.github.io/web-animation-game/](https://vasylpryimakdev.github.io/web-animation-game/)

## Features

### Character Animation

- **Idle Animation**: 8-frame sprite animation with smooth transitions
- **Jump Mechanics**: Realistic jumping with shadow scaling for depth perception
- **Animation States**: Proper state management prevents animation conflicts

### Parallax Scrolling

- **Multi-layer System**: Three depth layers creating realistic perspective
  - Background layer (slowest movement)
  - Street layer (base movement speed)
  - Foreground layer (fastest movement)
- **Continuous Motion**: Infinite linear animations for smooth scrolling

### Dynamic Vehicle System

- **Randomized Cars**: Vehicles spawn with varying speeds (200ms - 4200ms duration)
- **Rotating Wheels**: Realistic wheel rotation synchronized with car movement
- **Smart Spawning**: Prevents overlapping vehicles with state-aware generation
- **Automatic Cleanup**: DOM elements removed after animation completion

### Interactive Controls

- **Arrow Up**: Make character jump
- **Arrow Right**: Increase animation speed (up to 3x)
- **Arrow Left**: Decrease animation speed (down to 0.8x)
- **Space**: Pause/resume all animations

### Advanced Features

- **Auto-deceleration**: Animations gradually slow down every 5 seconds
- **Global Animation Control**: Pause/resume affects all scene elements
- **Speed Limits**: Prevents unrealistic animation speeds
- **State Management**: Intelligent animation state checking

## Technical Implementation

### Web Animations API

- Character sprite animation using `steps()` easing
- Parallax layers with different movement speeds
- Dynamic car generation and animation
- Synchronized shadow scaling during jumps

### CSS Architecture

- Modular component styling
- CSS custom properties for responsive sizing
- Pseudo-element animations for rotating wheels
- Optimized positioning and layering

### JavaScript Features

- Async/await for animation sequencing
- Dynamic DOM manipulation
- Event-driven architecture
- Performance-optimized animation loops

## File Structure

```
├── index.html          # Main HTML structure
├── styles.css          # Styling and animations
├── script.js           # Interactive functionality
├── assets/             # Image assets
│   ├── cloud1.png
│   ├── cloud2.png
│   ├── s1.png          # Background layer
│   ├── s2.png          # Foreground layer
│   ├── line.png        # Street lines
│   ├── 7888220.png     # Character sprite
│   ├── car.png         # Vehicle sprite
│   └── wheel.png       # Wheel sprite
└── README.md           # This file
```

## Controls

| Key   | Action       |
| ----- | ------------ |
| ↑     | Jump         |
| →     | Speed up     |
| ←     | Slow down    |
| Space | Pause/Resume |

## Browser Compatibility

- Chrome 36+
- Firefox 48+
- Safari 13.1+
- Edge 79+

## Getting Started

1. Clone the repository
2. Open `index.html` in a modern web browser
3. Use keyboard controls to interact with the animation

## Animation Details

### Character

- **Idle**: 8-frame cycle, 1000ms duration
- **Jump**: 500ms duration, 2 iterations, alternate direction
- **Shadow**: Scales to 1.15x during jump for depth effect

### Parallax Layers

- **Street**: 12-second base duration
- **Background**: 24-second duration (2x slower)
- **Foreground**: 18-second duration (1.5x faster)

### Vehicles

- **Spawn Rate**: Random intervals (0-4 seconds)
- **Speed Range**: 200ms to 4200ms cross-screen duration
- **Wheels**: Continuous rotation, 4x faster than car movement

---

Built with modern web technologies showcasing advanced animation techniques and interactive user experiences.
