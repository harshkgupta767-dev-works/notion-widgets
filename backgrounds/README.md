# Scenic Pomodoro — background library

Backgrounds for `widget-pomodoro-scenic.html` are organised by **motion category**.
Motion *is* the category: picking a background auto-applies that category's motion.

| Folder | Category | Motion | Use for |
|---|---|---|---|
| `panlr/` | Pan → | slow left→right pan | **wide / panoramic** images (need horizontal room) |
| `panrl/` | Pan ← | slow right→left pan | **wide / panoramic** images |
| `zoom/`  | Zoom | slow zoom in/out | standard 16:9 images |
| `ken/`   | Ken Burns | zoom + drift | standard 16:9 images |
| `still/` | Cinemagraph | none (static) | **muted, seamless-loop video** (.mp4 / .webm) |

## Image specs
- 16:9 landscape. `zoom`/`ken`: 1920×1080+. `panlr`/`panrl`: wider (e.g. 2560×1080) reads best, since the frame pans.
- JPG/WebP, keep each well under ~500 KB so several widgets stay light.

## Video specs (`still/`)
- 1920×1080, 6–10 s **seamless loop**, **muted**, **< 8 MB**, MP4 (H.264) — optional `.webm` + a poster `.jpg` (shown instantly + for reduced-motion).

## Adding a background
1. Drop the file in the matching folder.
2. In `widget-pomodoro-scenic.html`, add an item to that category's `items[]` in `LIBRARY`:

```js
// image
{ id:'meadow', name:'Meadow', img:'backgrounds/panlr/meadow.jpg' }
// video (still/cinemagraph)
{ id:'rain', name:'Rain', video:'backgrounds/still/rain.mp4', webm:'backgrounds/still/rain.webm', poster:'backgrounds/still/rain.jpg' }
```

The picker auto-populates from `LIBRARY`. Items may also be a `css:` gradient or inline `svg:` (the six built-ins live in the `RAW` map and are referenced by the library).

> Tip: paste any image/video URL into the **Custom background** field in settings to preview without committing files. When custom is on, a small motion picker appears (since an arbitrary image has no inherent motion).
