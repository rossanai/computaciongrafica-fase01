# 🎯 3D Parabolic Cannon Simulator

This project is a custom 3D graphics engine developed for a Computer Graphics course. It features an interactive 3D rendering environment built entirely through code, focusing on simulating parabolic projectile physics, spatial collision detection, and hierarchical matrix transformations without relying on pre-built commercial game engines.

## 🚀 Core Features

* **Physics & Kinematics:** Real-time parabolic trajectory simulation. It implements gravity and *delta time* calculations to ensure the projectile's flight remains consistent and completely independent of the frame rate (FPS).
* **Transformation Hierarchy:** Articulated turret modeling managed through mathematical matrices. The cannon barrel includes precise rotation constraints (strict clamping between 5° and 90°).
* **3D Collision Detection:** Custom collision system based on Euclidean distance calculations across the X, Y, and Z axes to register exact impacts between the dynamic projectile and static targets in 3D space.
* **Procedural Primitives:** Construction of 3D geometries (optimized topology spheres and rectangular prisms) by calculating vertices and polygons programmatically from scratch.
* **Dynamic In-Game UI:** Power indicator integrated directly into the 3D world (status bars rendered on the model) that reacts to real-time keyboard events.

## 🎮 Controls

* **Left / Right Arrows:** Translate turret laterally across the field limits.
* **Up / Down Arrows:** Adjust cannon pitch angle (clamped between 5° and 90°).
* **1, 2, 3 / F:** Change launch power level (visually indicated by status bars).
* **Spacebar:** Fire projectile (single-projectile lock active during flight).
* **R:** Reset active targets, turret position, and projectile state.

## 🛠️ Tech Stack & Requirements

* **Language:** TypeScript
* **Graphics:** 3D Projection Math / WebGL2
* **Environment:** Vite / Node.js 18+

## ⚙️ How to Run

1. Install dependencies:
   ```bash
   npm install
   
Start development server:
npm run dev

Open http://localhost:5173 in your browser.
