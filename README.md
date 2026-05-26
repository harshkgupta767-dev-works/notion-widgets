# Notion Widgets

Custom widgets built for the **Dark Academia XP Student Planner** Notion template.  
Hosted on GitHub Pages — embed using Notion's `/embed` block.

---

## 🔗 Widget Links

| Widget | Link |
|--------|------|
| 🕰 Flip Clock | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-flip-clock.html |
| ⏱ Pomodoro Timer | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-pomodoro.html |
| 🎵 Music Player | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-music-player.html |
| 🌧 Matrix Rain | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-matrix.html |

---

## 📐 Recommended Embed Sizes

| Widget | Mode | Width | Height |
|--------|------|-------|--------|
| Flip Clock | Standard (4-tile) | 500px | 220px |
| Flip Clock | Compact (2-tile) | 320px | 200px |
| Pomodoro Timer | — | 420px | 620px |
| Music Player | Full (Spotify / YouTube) | 420px | 460px |
| Music Player | Compact (Spotify only) | 420px | 140px |
| Matrix Rain | — | any | any |

---

## 📁 Files

- `widget-flip-clock.html` — Flip clock with Standard (4-tile) and Compact (2-tile) modes. Settings include:
  - **Fonts** — Anton, Bebas Neue, Oswald, JetBrains Mono, Squada One, Chakra Petch
  - **Tile presets** — 7 built-in colour presets (Charcoal, Obsidian, Nord, Coffee, Cyber, Gold, Parchment) + custom colour picker
  - **Colour pickers** — separate controls for tile, number, and date/day colours; the **number** and **date** swatch palettes adapt to the selected theme so the colours always contrast the background they sit on (custom colour stays available in both themes)
  - **Motion** — Smooth, Mechanical, Minimal, or Instant flip animation with physics-quality 3D perspective, depth gradient shading, and cast drop shadows on the rotating flap
  - **Theme** — Light or Dark
  - **Format** — 12 HR or 24 HR
  - **Display** — Day & Date, Date only, Day only, or None
  - **Zoom** — 50 – 150 % scale
  - Responsive layout for narrow embeds; gear icon auto-adapts to tile brightness

- `widget-pomodoro.html` — Pomodoro timer with focus/break cycles and session tracking. Settings include:
  - **Theme** — Dark or Light
  - **Widget Color** — custom background colour picker
  - **Accent Color** — custom accent colour picker
  - **Glow** — adjustable ring glow intensity slider
  - **Ring Style** — Smooth or Sharp progress ring
  - **Durations** — Focus, Short Break, and Long Break lengths (minutes)
  - **Sessions** — number of sessions per cycle (default 4)
  - **Auto-advance** — automatically start the next session/break
  - **Sound** — toggle notification sound on/off, with volume slider
  - **Zoom** — 50 – 150 % scale
  - Session history panel with editable past entries; dots indicator shows cycle progress

- `widget-music-player.html` — Embedded Spotify or YouTube player. Settings include:
  - **Theme** — Minimal, Dark, OLED, Mono
  - **Ambient Glow** — pulsing glow effect on the player card
  - **Zoom** — 50 – 150 % scale
  - **Link** — paste any Spotify or YouTube URL to load it
  - **Spotify View** — toggle between Compact (80px) and Full (400px) player
  - **Presets** — save and manage custom playlist/track presets with labels; recent links history
  - Switches automatically between Spotify and YouTube embed based on the pasted URL

- `widget-matrix.html` — Fullscreen Matrix-style digital rain. Settings include:
  - **Theme** — Dark or Light canvas background
  - **Style** — Bold or Normal characters
  - **Characters** — Matrix (カナ), Alpha (ABC), Binary (01), Digits (123), Glitch (!@#), or Chaos — picked from a tile grid that previews a sample character
  - **Colour** — 6 theme-aware preset swatches (bright tones on the dark theme, deeper tones on the light theme) plus a full HSV custom colour picker; switching theme migrates the choice by index so the rain stays visible
  - **Speed** — 1 – 4 (step 0.25)
  - **Font Size** — 8 – 20 px (step 1)
  - **Trail Length** — 2 – 14 (step 1)
  - Settings panel opens in the top-left corner with no overlay so live changes are visible behind it
  - Fills any embed size; settings accessible via gear icon
