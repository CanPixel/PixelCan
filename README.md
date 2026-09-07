# PixelCan (CAN)

**PixelCan** is an HTML5 2D pixel-art web game created with the [Construct 2](https://www.scirra.com/construct2) game engine.

---

## 🎮 Overview

- **Engine:** Construct 2 HTML5 Game Engine
- **Canvas Resolution:** 1000 × 500 (scales dynamically to viewport)
- **Visuals:** Custom 2D pixel-art spritesheets and lighting effects
- **Platforms:** Web Browsers (Desktop & Mobile with touch support)

---

## 📁 Project Structure

```text
pixelcan/
├── images/                 # Spritesheets, textures, UI elements, and character animations
├── c2runtime.js            # Construct 2 game engine runtime logic
├── corporate.css           # Custom font styling
├── corpo___.ttf            # Font file used in the game
├── icon-*.png              # Web and mobile application icons (16px to 256px)
├── index.html              # Main HTML entry point rendering the game canvas
├── info.can                # Leaderboard / metadata configuration
├── jquery-3.7.1.min.js     # jQuery library for DOM manipulation and runtime setup
├── loading-logo.png        # Game loading screen logo
├── offline.appcache        # Offline caching manifest for PWA/HTML5 offline support
└── README.md               # Project documentation
```

---

## 🚀 Getting Started / How to Run

Because modern browsers enforce CORS and security restrictions on the `file:///` protocol, the game must be served via a local web server.

### Option 1: Using Python
```bash
# Python 3
python3 -m http.server 8000
```
Then open [http://localhost:8000](http://localhost:8000) in your browser.

### Option 2: Using Node.js / `npx`
```bash
npx serve .
```

### Option 3: VS Code / IDE Extensions
Use an extension such as **Live Server** to run `index.html` on a local development server.

---

## ⚙️ Notes

- **jQuery Reference:** Ensure that the `<script src="...">` tag in `index.html` matches the jQuery file version in the project root (`jquery-3.7.1.min.js`).
- **Offline Support:** The game includes `offline.appcache` for offline web app capabilities.
