# Brick Vector

A polished Breakout / brick-breaker clone built entirely with vanilla JavaScript and the Canvas API — no frameworks, no build step, no external dependencies. The whole game (HTML, CSS, and JS) lives in a single `index.html` file.

This project demonstrates a fixed-timestep game-loop architecture decoupled from rendering, device-pixel-ratio-aware responsive canvas drawing, real angle-reflection paddle physics, layered keyboard/mouse/touch input handling, multi-level progression with escalating difficulty, and small accessibility touches (reduced-motion support, focus-visible states, live-region status updates) alongside persisted local state.

## Features
- Smooth fixed-timestep game loop (requestAnimationFrame + accumulator) with a clamped catch-up loop to avoid the spiral of death
- Responsive, device-pixel-ratio-aware canvas rendering that fits any screen size
- Real angle-reflection paddle physics — where the ball strikes the paddle determines its bounce angle, with steeper deflection near the edges
- Keyboard (arrow keys / A-D) and touch/mouse (drag-to-follow) paddle controls
- Five distinct hand-designed brick layouts (full grid, diamond gap, checkerboard, gated columns, X pattern) that cycle with increasing ball speed and reinforced (2-hit) bricks on later passes
- Row-based scoring, a 3-life system, and level-clear detection
- Persistent high score via `localStorage`
- Clean start, pause, level-clear, and game-over screens with an in-canvas HUD
- Reduced-motion support (skips decorative particle bursts and shortens transition timing) and keyboard-focus-visible styling

## Run it
Just open `index.html` in a browser — no build step, no install.

## Live version
TBD — will be added after deployment
