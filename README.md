# Newton's Cradle — Physics Simulation

A browser-based Newton's cradle demonstration built with **Matter.js** and **p5.js**. Five suspended balls are connected to a support using physics constraints.

## Features

- Five moving circular physics bodies
- A static overhead support
- Rope constraints connecting the balls to the support
- A keyboard-controlled force that starts the motion

## How to run

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Start a local HTTP server:

   ```bash
   python -m http.server 8000
   ```

4. Visit **http://localhost:8000/** in your browser.

Python is only used here to serve the static files. The repository includes its referenced JavaScript libraries, so no npm install or build step is needed.

## Control

**Up arrow** — Apply a force to the first ball to start the motion.

## File structure

- `index.html` — Browser entry point
- `sketch.js` — Simulation setup, rendering and keyboard input
- `bob.js` — Physics body for each ball
- `rope.js` — Physics constraints and rope drawing
- `roof.js` — Fixed support
- `matter.js`, `p5.js`, `p5.play.js` — Bundled libraries

## Notes

This is a simple classroom-style physics demonstration with a fixed 800 × 600 canvas, not a precision scientific simulator.
