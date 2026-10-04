# Real-Time MLB Play Drinking Game

A standalone Progressive Web App (PWA) that connects directly to the official **MLB Stats API** (`https://statsapi.mlb.com`) to track real-time play-by-play events during baseball games, assign drinks based on customizable rules, and trigger animated 8-bit retro pixel art and synth sound effects!

---

## Key Features

- **Real-Time MLB API Polling**: Connects directly to MLB's live game feed (`/api/v1.1/game/{gamePk}/feed/live`) with fast 3-second polling. Responds to plays as soon as official data updates.
- **Complete MLB Play-by-Play Feed**: Displays detailed official MLB play descriptions for all plays (outs, hits, walks, scoring events), cleanly separating non-drink plays from drink-assigning events.
- **Standardized Pixel Drink Badges**: Every drink play features a custom retro pixel SVG beer mug badge displaying the exact numeric drink count (e.g. `1`, `2`, `6`).
- **30 FPS Retro Canvas Pixel Art**: Self-contained, 30 FPS retro stadium canvas graphics with twinkling night stars, floodlights, and custom event scenes:
  - **Strikeouts / Homeruns / Stolen Bases / Errors / Walks / Hit By Pitch / Rain Delays**: Animated 8-bit retro arcade scenes & banners.
- **Web Audio Chiptune SFX**: 8-bit sound synthesizers (whiff, buzzer, fanfare, drink chime) built directly in JS with no external audio file dependencies.
- **Customizable Ruleset Editor**: Edit drink amounts per play type in real time with responsive row cards and input fields supporting custom text (`Finish Drink`, `1 per base`, `Take a shot`).
- **Game Drink Summary**: Accumulates total assigned drinks per event category (e.g. total drinks assigned from Strikeouts, Hits, Home Runs, Errors, etc.).
- **Demo Play Mode**: Preview all pixel art animations, sound effects, and drink triggers anytime without needing a live game.

---

## Customizable Ruleset

The table below outlines the **default drinking ruleset** configured in the app. All drink assignments are fully customizable in real time via the **RULES** editor in the app header (and live-synced in the **Current Ruleset** panel on the main page):

| Play Event | Drink Assignment |
| :---: | :---: |
| **Strikeout (K)** | 1 Drink |
| **Walk (BB)** | 1 Drink |
| **Single (1B)** | 2 Drinks |
| **Double (2B)** | 3 Drinks |
| **Triple (3B)** | 4 Drinks |
| **Homerun (HR)** | **FINISH YOUR DRINK!** |
| **Hit By Pitch (HBP)** | 5 Drinks |
| **Double Play (DP)** | 2 Drinks |
| **Triple Play (TP)** | 5 Drinks |
| **Balk** | 5 Drinks |
| **3rror (Fielding Error)** | 3 Drinks |
| **Stolen Base** | 1 Drink per base |
| **New Inning** | 1 Drink |
| **Rain Out / Delay** | **TAKE A SHOT!** |

*All rules can be customized live using the **RULES** button in the app header!*
