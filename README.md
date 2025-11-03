# Cub3D

Cub3D is a minimalist 3D engine inspired by classic shooters like *Wolfenstein 3D*.  
It renders a pseudo-3D world from a 2D map using the **raycasting** technique and the **DDA algorithm** for efficient wall detection.

Built entirely in **C** with **MiniLibX** for rendering, it features:
- Real-time movement and camera rotation
- Collision detection
- Textured wall rendering (if you added that)
- Simple, optimized rendering loop

The project explores how early 3D games simulated depth and perspective with limited resources — from calculating ray directions to projecting walls on screen.

This was a deep dive into graphics programming, vector math, and low-level game loops.

*(Originally inspired by the 42 project “Cub3D,” later expanded and refined for personal learning.)*

 ---

 ## 🕹 How to Run

### 1. Clone the repository

### 2. Build the project
cd Cub3D
make

### 3. Run the program
./cub3D maps/example.cub

---
🎮 Controls

| Key                    | Action                           |
| ---------------------- | -------------------------------- |
| **W / S**              | Move forward / backward          |
| **A / D**              | Strafe left / right              |
| **← / →**              | Rotate camera left / right       |
| **ESC**                | Exit the game                    |

---
🧱 Textures

Cub3D supports custom wall textures.
You can use any .xpm image file as a texture by placing it inside the textures/ directory and updating your map configuration.

Example snippet from a map file:

NO ./textures/stone.xpm
SO ./textures/brick.xpm
WE ./textures/wood.xpm
EA ./textures/metal.xpm

| Prefix | Meaning           |
| ------ | ----------------- |
| **NO** | North-facing wall |
| **SO** | South-facing wall |
| **WE** | West-facing wall  |
| **EA** | East-facing wall  |
