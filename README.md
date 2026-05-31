# Notion Widgets

Custom widgets built for the **Dark Academia XP Student Planner** Notion template.  
Hosted on GitHub Pages — embed using Notion's `/embed` block.

---

## 🔗 Widget Links

| Widget | Link |
|--------|------|
| 🌦 Weather | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-weather.html |
| 🕰 Flip Clock | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-flip-clock.html |
| ⏱ Pomodoro Timer | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-pomodoro.html |
| 🌄 Scenic Pomodoro | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-pomodoro-scenic.html |
| 🎵 Music Player | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-music-player.html |
| 🌧 Matrix Rain | https://harshkgupta767-dev-works.github.io/notion-widgets/widget-matrix.html |

---

## 📐 Recommended Embed Sizes

| Widget | Mode | Width | Height |
|--------|------|-------|--------|
| Weather | Full (hourly + 7-day) | 520px | 300px |
| Weather | Compact (current only) | 340px | 190px |
| Flip Clock | Standard (4-tile) | 500px | 220px |
| Flip Clock | Compact (2-tile) | 320px | 200px |
| Pomodoro Timer | — | 420px | 620px |
| Scenic Pomodoro | — | 640px | 360px |
| Music Player | Full (Spotify / YouTube) | 420px | 460px |
| Music Player | Compact (Spotify only) | 420px | 140px |
| Matrix Rain | — | any | any |

---

## 📁 Files

- `widget-weather.html` — Live weather widget powered by Open-Meteo (free, no API key, CORS-enabled). Settings include:
  - **Location** — city search plus a multi-city switcher: save up to 5 cities and switch instantly via tabs on the widget; each city's data is cached so switching back is instant, with a silent background refresh when stale
  - **Units** — °C or °F
  - **Forecast Days** — 3, 5, or 7 day outlook
  - **Layout** — Full (current conditions + scrollable hourly strip + daily forecast) or Compact (current conditions only)
  - **Day Labels** — Short (Mon) or Full (Monday)
  - **Theme** — Light or Dark, with per-theme background and text colour palettes plus full HSV custom colour pickers
  - **Display toggles** — Ambient gradient background, Hourly strip, Air quality (AQI), Feels-like temp, Rain chance, Forecast rain %, Dates, Condition text, Animated icons, Greyscale icons
  - **Zoom** — 50 – 160 % scale
  - **Multi-model consensus** — blends five forecast models (ECMWF, GFS, ICON, GEM, JMA) and takes the median of every value, so one outlier model can't show a false storm
  - **Smart rain detection** — weather codes are reconciled against actual precipitation amount (mm) and cloud cover, so dramatic icons and the rain chip only appear when rain is genuinely forecast
  - Custom inline-SVG weather icons (clear/cloud/fog/drizzle/rain/snow/thunder, day & night variants) with optional CSS animation; location-local clock; "Weather by Open-Meteo" attribution (CC BY 4.0)

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

- `widget-pomodoro-scenic.html` — Scenic Pomodoro inspired by studywithme.io: a full-bleed animated background with minimal white UI floating on top (no card or border). Fonts are Fredoka (timer digits) + Quicksand (UI). Settings include:
  - **Scene** — 6 self-contained backgrounds with no image files (Sunset, Ocean, Forest, Night, Sakura, Noir), built from inline SVG art and CSS gradients; Night adds a generated star field
  - **Custom background** — paste any image URL and toggle **Use custom image** to use it instead of a built-in scene
  - **Motion** — Ken Burns (zoom + drift), Pan left → right, Pan right → left, Slow zoom, or Static
  - **Overlay darkness** — 0 – 60 % tint over the scene for text legibility
  - **Zoom** — 70 – 130 % scale of the floating UI
  - **Durations** — Pomodoro, Short Break, and Long Break lengths (minutes)
  - **Sequence** — Pomodoros before a long break (2 – 8) and an **Auto-start next** toggle
  - **Sound** — Bell, Chime, Soft, or None alert (Web Audio, no files), with a play-on-end toggle, volume slider, and Test button
  - Timestamp-based countdown that stays accurate across tab throttling; session dots under the mode pills fill as focus sessions complete; dark settings modal with General / Timers / Sounds tabs

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
