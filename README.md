# ⚾🍺 Real-Time MLB Play Drinking Game

A standalone Progressive Web App (PWA) that connects directly to the official **MLB Stats API** (`https://statsapi.mlb.com`) to track real-time play-by-play events during baseball games, assign drinks based on customizable rules, and trigger animated 8-bit retro pixel art and synth sound effects!

---

## 🌟 Key Features

- **⚡ Real-Time MLB API Polling**: Connects directly to MLB's live game feed (`/api/v1.1/game/{gamePk}/feed/live`) with fast 3-second polling. Responds to plays as soon as official data updates.
- **🎨 Retro 8-Bit Canvas Pixel Art**: Self-contained, procedural retro canvas graphics for key drink events:
  - **Strikeouts / Hits / Homerun / Rain Out**: Animated retro scenes & banners.
- **🔊 Web Audio Chiptune SFX**: 8-bit sound synthesizers (whiff, buzzer, fanfare, drink chime) built directly in JS with no external audio file dependencies.
- **⚙️ Customizable Ruleset**: Edit drink amounts per play type in real-time via the in-app Rules editor.
- **📱 PWA & Standalone Support**: Installable on iPhone, Android, or Desktop. Works offline and from a single file/URL!
- **🎮 Demo Play Mode**: Preview all pixel art animations, sound effects, and drink triggers anytime without needing a live game.

---

## 🍻 Default Drinking Ruleset

| Play Event | Drink Assignment |
| :--- | :--- |
| **Strikeout (K)** | 🍺 1 Drink |
| **Walk (BB)** | 🍺 1 Drink |
| **Single (1B)** | 🍺 2 Drinks |
| **Double (2B)** | 🍺 3 Drinks |
| **Triple (3B)** | 🍺 4 Drinks |
| **Homerun (HR)** | 🍺 **FINISH YOUR DRINK!** |
| **Hit By Pitch (HBP)** | 🍺 5 Drinks |
| **Double Play (DP)** | 🍺 2 Drinks |
| **Triple Play (TP)** | 🍺 5 Drinks |
| **Balk** | 🍺 5 Drinks |
| **3rror (Fielding Error)** | 🍺 3 Drinks |
| **Stolen Base** | 🍺 1 Drink per base |
| **New Inning** | 🍺 1 Drink |
| **Rain Out / Delay** | 🥃 **TAKE A SHOT!** |

*All rules can be customized live using the **⚙️ RULES** button in the app header!*

---

## 🚀 How to Run & Share with Friends

### Option 1: Direct File Sharing (Zero Server Required)
Simply send the `index.html` file to your friends! They can open `index.html` directly in Chrome, Safari, Edge, or Firefox on mobile or desktop.

### Option 2: Local Web Server (For PWA Installation)
To test PWA installation or run locally:
```bash
# Using Node.js (http-server)
npx http-server -p 8080

# Then open http://localhost:8080 in your browser!
```

### Option 3: Host Online (Free & Instant)
Host the workspace folder on **GitHub Pages**, **Vercel**, or **Netlify**:
1. Upload `index.html`, `manifest.json`, and `sw.js` to a GitHub repo.
2. Enable **GitHub Pages** in Repository Settings.
3. Share the generated link with your friends! Everyone can select the same game and get identical real-time play alerts.
