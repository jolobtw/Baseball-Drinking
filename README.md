# Retro Sports Real-Time Drinking Game

A standalone Progressive Web App (PWA) that connects directly to official live stats APIs—**MLB Stats API** (`https://statsapi.mlb.com`) and **NFL ESPN Stats API** (`https://site.api.espn.com`)—to track real-time play-by-play events during live games, assign drinks based on customizable rules, and trigger animated 8-bit retro pixel art and synth sound effects!

---

## Key Features

- **Multi-Sport Support (MLB & NFL)**: Seamlessly switch between MLB Baseball and NFL Football with a dedicated sport selector screen and dynamic theme styling.
- **Real-Time Stats API Polling**: Connects directly to MLB and NFL live game feeds with fast 3-second polling to update play feeds in real time.
- **Complete Play-by-Play Feed**: Displays detailed official play descriptions for all plays, cleanly highlighting drink-assigning events with custom retro pixel badges.
- **Standardized Pixel Drink Badges**: Every drink play features a custom retro pixel SVG beer mug badge displaying the exact numeric drink count (e.g. `1`, `2`, `3`, `6`).
- **30 FPS Retro Canvas Pixel Art**: Self-contained retro stadium canvas graphics with stadium floodlights and custom 8-bit event animations:
  - **MLB Events**: Strikeouts, Homeruns, Stolen Bases, Errors, Walks, Hit By Pitch, and Rain Delays.
  - **NFL Events**: Touchdowns, Interceptions, Fumbles, Field Goals, First Downs, Timeouts, Quarter Changes, and Safeties.
- **Web Audio Chiptune SFX**: Built-in 8-bit sound synthesizers (whiff, buzzer, fanfare, chime, referee whistle) with zero external audio file dependencies.
- **Customizable Ruleset Editor**: Edit drink amounts per play type in real time for both MLB and NFL rulesets.
- **Game Drink Summary**: Tracks and accumulates total assigned drinks per event category.
- **Demo Play Mode**: Preview pixel art animations, sound effects, and drink triggers anytime without needing a live game.

---

## Customizable Rulesets

The tables below outline the **default drinking rulesets** for MLB and NFL games. All drink assignments are fully customizable in real time via the **RULES** editor in the app header:

### MLB Baseball Ruleset

| Play Event | Drink Assignment |
| :---: | :---: |
| Strikeout (K) | 1 Drink |
| Walk (BB) | 1 Drink |
| Single (1B) | 2 Drinks |
| Double (2B) | 3 Drinks |
| Triple (3B) | 4 Drinks |
| Homerun (HR) | FINISH YOUR DRINK! |
| Hit By Pitch (HBP) | 5 Drinks |
| Double Play (DP) | 2 Drinks |
| Triple Play (TP) | 5 Drinks |
| Balk | 5 Drinks |
| 3rror (Fielding Error) | 3 Drinks |
| Stolen Base | 1 Drink per base |
| New Inning | 1 Drink |
| Rain Out / Delay | TAKE A SHOT! |

<br>

### NFL Football Ruleset

| Play Event | Drink Assignment |
| :---: | :---: |
| Touchdown (TD) | FINISH YOUR DRINK! |
| Interception (INT) | 3 Drinks |
| Fumble Turnover | 2 Drinks |
| Field Goal (FG) | 2 Drinks |
| First Down | 1 Drink |
| Timeout | 1 Drink |
| Quarter Change | 1 Drink |
| Safety | TAKE A SHOT! |

<br>

*All rules can be customized live using the **RULES** button in the app header!*
