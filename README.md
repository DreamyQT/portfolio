# The Analyst Studio — Interactive 3D Portfolio

**Live site:** [https://dreamyqt.github.io/portfolio/](https://dreamyqt.github.io/portfolio/)

An interactive 3D portfolio built as a bright, modern analyst's studio. Orbit the room, hover over objects to see what's interactive, and click around to explore — the monitor opens my About panel, the whiteboard holds my projects, the bookshelf my skills, the corkboard my contact links, and the document tray my resume. There's also a working light switch on the wall: flip it and the room goes dark, a moon and starfield appear outside, and spotlights pick out everything clickable.

## Built with

- **Three.js (WebGL)** — the entire scene is procedural: every desk, shelf, plant, and object is generated in code. No 3D model files, no textures, no assets.
- **Vanilla JavaScript** — camera controls, raycast-based hover/click interaction, the day/night transition, and animations (real-time wall clock, coffee steam, dust motes, star twinkle).
- **Canvas API** — the dashboard on the monitor, the whiteboard sketches, the pinned corkboard notes, the framed certificates, and the day/night skies are all drawn programmatically to canvas textures.
- **HTML/CSS** — the info panels, loading screen, and light/dark UI theming.

No frameworks, no build step, no dependencies to install — the whole site is a single `index.html`.

## Features

- Smooth camera fly-in with an animated loading screen
- Six clickable objects with hover highlighting, each opening a themed info panel
- Day/night mode via a 3D light switch, with gallery spotlights guiding visitors to the interactive objects
- Mobile-responsive with performance scaling (lower pixel ratio, shadows disabled, fewer particles on small screens)
- Respects `prefers-reduced-motion`

## Running locally

Clone the repo and open `index.html` in a browser — that's it. For live-reload while editing, use the VS Code **Live Server** extension. An internet connection is required (Three.js and fonts load from CDNs).

## Structure

Everything lives in one file, organized top to bottom:

| Section | What's there |
|---|---|
| `<style>` | Theme variables, panel styling, loading screen, dark-mode overrides |
| `<template>` blocks | All text content (About, Projects, Skills, Contact, Resume) |
| `<script type="module">` | Scene setup, canvas textures, 3D object builders (each labeled), interaction, and the animation loop |

## Contact

- **Email:** sing8465@mylaurier.ca
- **LinkedIn:** [linkedin.com/in/devesh-singarh-089327379](https://www.linkedin.com/in/devesh-singarh-089327379)
- **GitHub:** [@DreamyQT](https://github.com/DreamyQT)
