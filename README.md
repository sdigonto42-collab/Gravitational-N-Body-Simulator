# 2D Interactive Gravitational N-Body Simulator

An interactive physics visualizer built with HTML5 Canvas and JavaScript to simulate multi-body gravitational interactions in 2D space.

## 🚀 Live Demo
[Click here to run the simulation live in your browser](

## 📌 Features
- **N-Body Gravitational Physics:** Real-time computation of gravitational vectors between multiple celestial bodies.
- **Orbital Path Tracking:** Fading trajectory trails showing past planetary motion.
- **Mobile Touch Controls:** Tap and drag anywhere on the canvas to launch custom bodies with initial velocity vectors.
- **Parameter Controls:** Dynamic adjustment of the universal gravitational constant ($G$) and preset solar configurations.

## 🧮 Theoretical Foundation
The simulation calculates mutual gravitational attraction using Newton's Law of Universal Gravitation:

$$F = G \frac{m_1 m_2}{r^2 + \epsilon}$$

Where:
- $G$ is the gravitational constant.
- $r = \sqrt{\Delta x^2 + \Delta y^2}$ is the Euclidean distance between two bodies.
- $\epsilon$ is a softening parameter used to avoid division by zero during close encounters.

Position and velocity are updated each frame using Euler Integration:
$$v_{x, \text{new}} = v_x + a_x \cdot \Delta t$$
$$x_{\text{new}} = x + v_x \cdot \Delta t$$

## 🛠️ Tech Stack
- **Language:** JavaScript (ES6)
- **Rendering:** HTML5 2D Canvas API
- **Styling:** CSS3
