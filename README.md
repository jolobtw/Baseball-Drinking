# Retro Sports Real-Time Drinking Game

A standalone Progressive Web App (PWA) that connects directly to official live stats APIs—**MLB Stats API** (`https://statsapi.mlb.com`) and **NFL ESPN Stats API** (`https://site.api.espn.com`)—to track real-time play-by-play events during live games, assign drinks based on customizable rules, and trigger animated 8-bit retro pixel art and synth sound effects!

---

## Key Features

- **Multi-Sport Support (MLB & NFL)**: Seamlessly switch between MLB Baseball and NFL Football with a dedicated sport selector screen and dynamic theme styling.
- **Real-Time Stats API Polling**: Connects directly to MLB and NFL live game feeds with fast 3-second polling to update play feeds, scores, live base runner indicators, and count dots in real time.
- **Revamped MLB Scoreboard**: Sleek, tightly grouped retro base runner diamond (with 1st/2nd/3rd base glow and home plate) positioned right next to glowing Ball / Strike / Out LED count indicators.
- **Complete Play-by-Play Feed**: Displays detailed official play descriptions for all plays, cleanly highlighting drink-assigning events with custom retro pixel badges.
- **Standardized Pixel Drink Badges**: Every drink play features a custom retro pixel SVG beer mug badge displaying the exact numeric drink count (e.g. `1`, `2`, `3`, `6`).
- **Static Retro Canvas Pixel Art**: Self-contained 8-bit retro stadium canvas graphics with stadium floodlights and distinct static play illustrations (with zero text repetition across the pop-up modal):
  - **MLB Events**: Strikeouts (Red pixel 'K'), Homeruns (Rainbow arc in stars), Stolen Bases (Sliding shoe into base bag), Errors (Orange warning triangle & dropped ball), Walks (4-ball count dots), Hit By Pitch (Red target reticle), Rain Delays, and Base Hits.
  - **NFL Events**: Touchdowns (Yellow goalposts & TD ref signal), Interceptions (Leaping DB catch & lightning bolts), Fumbles (Bouncing football & impact burst), Field Goals (Uprights with centered football), Big Plays (Speed trail runner), First Downs (10-yard chain poles & arrow), Timeouts (Stopwatch clock icon), Quarter Changes (Stadium LED box), and Safeties (Safety shield).
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
| Big Play (10+ Yds) | 1 Drink per 10 yards gained |
| First Down | 1 Drink |
| Timeout | 1 Drink |
| Quarter Change | 1 Drink |
| Safety | TAKE A SHOT! |

<br>

*All rules can be customized live using the **RULES** button in the app header!*
