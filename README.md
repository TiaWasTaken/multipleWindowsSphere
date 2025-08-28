# Multi-Window 3D Scene with Three.js

## Overview
This project explores how to render and synchronize a 3D environment across several browser windows using **Three.js** in combination with **localStorage**.  
It’s aimed at developers who want to experiment with unconventional graphics setups and advanced browser window coordination.

---

## Key Features
- Build and display interactive 3D content with Three.js  
- Keep multiple browser windows in sync, sharing the same scene state  
- Track, update, and remove windows dynamically through localStorage  

---

## Getting Started
Download or clone the repository, then simply open `index.html` in your browser.  
The scene will render automatically and will react to the presence of additional windows you open.

---

## Installation
Clone the repository and open `index.html` in your browser to start exploring the 3D scene:

```bash
git clone https://github.com/TiaWasTaken/multipleWindowsSphere.git
```

Start a server with python3 like this:

```bash
python3 -m http.server 8000
```

---

## Project Layout
- **index.html** → Loads the Three.js library, defines the page structure, and starts the main script  
- **WindowManager.js** → Handles communication between windows, keeping their state consistent  
- **main.js** → Sets up the 3D scene, manages window events, and drives the rendering loop  
- **three.r124.min.js** → The minified Three.js library powering the 3D graphics  

---

## How It Works
- **WindowManager.js** tracks each browser window, storing metadata (size, position, etc.) in `localStorage`.  
  When a window is moved, resized, opened, or closed, all active windows are updated accordingly.  
- **main.js** creates the scene with Three.js, listens for changes in window geometry, and animates objects to match the live state of all open windows.  

---

## Contributing
Suggestions and improvements are welcome!  
Fork the project, implement your ideas, and open a pull request.

---

## License
Released under the **MIT License** – free to use, modify, and share.

---

## Credits
- Thanks to the **Three.js developers** for their outstanding open-source 3D engine   
