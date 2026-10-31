# FauxOS

A simulated desktop operating system that runs entirely in the browser — one self-contained `index.html`, no build step.

## Run it

Open `index.html` in a modern browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## What's inside

- Windowed desktop with taskbar, Start menu, App Store, and My Files (saved to localStorage)
- FauxAuth sign-in: local accounts (PBKDF2-hashed passwords) and guest mode
- Browser: real web pages with tabs, back/forward, Google search, YouTube video links and editable start-page shortcuts (sites that forbid embedding open in a new tab)
- Apps: Code Lab, Camera, Oasis ambient scenes, background music player, screenshot and screen recording
- Games: Casino (slots, blackjack, roulette), Hop Rush, Spacewaves, Snake, and Blockwild (a WebGL voxel sandbox)
- Shared features (Chat, Clipcast video sharing) that use the claude.ai artifact runtime (`window.claude`); these only work on the published page and are unavailable when opened locally
