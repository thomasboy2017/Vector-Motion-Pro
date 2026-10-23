# Vecta Motion Pro

A single-file vector drawing and keyframe-animation studio for the browser. Open
`vecta-motion-pro.html` directly — there is no build step, package install, or server
required for the editor itself.

> Experimental / hobbyist project. It is not a replacement for Illustrator or Animate.
> Save important work as a project JSON file.

## Highlights

**Drawing**
- Rectangles, ellipses, lines, stars, polygons, brush strokes, multi-line text
- Multi-select (Shift-click or marquee), move/resize/rotate with 8 handles + rotation handle
- Align and distribute, layer reordering, lock/visibility, rename
- Snapping guides, grid, onion skin, zoom/pan/fit
- Solid or linear-gradient fills, strokes/dashes, corner radius
- Drop shadows, blur, blend modes
- Undo/redo, copy/cut/paste, Alt-drag duplicate, nudge with arrow keys

**Animation**
- Keyframes with 8 easing types, auto-key, onion skin
- Timeline zoom, scrubbing, keyframe retiming (drag diamonds), delete keyframes
- Copy/paste/reverse motion between objects
- Loop / once / ping-pong playback
- Full-screen preview

**Files & export**
- Save/open project JSON, autosave to local storage
- Import images (PNG/JPEG/WebP/GIF/SVG), PSD (best-effort layers), AI/PDF (first page raster)
- Export SVG, PNG, JPEG, WebP, sprite sheet (PNG), MP4 H.264/H.265 or WebM
- Command palette on `Ctrl/Cmd + K`
- Sample scene: **Neon Orbit**

## Quick start

1. Open the HTML file in a modern Chromium-based browser (Chrome/Edge recommended).
2. Press `R` and drag to draw a rectangle, or use the left toolbar.
3. Select it, open **Motion**, and click **Add keyframe at playhead**.
4. Scrub the timeline, move the object, then press **Play**.
5. Use **Export** for a still, sprite sheet, or video.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `V` `R` `E` `L` `S` `P` `T` `B` `X` `H` | Select, rect, ellipse, line, star, polygon, text, brush, eraser, pan |
| `Space` | Play / pause |
| `← ↑ → ↓` | Nudge 1 px (Shift = 10 px) |
| `,` / `.` | Previous / next frame |
| `Home` / `End` | First / last frame |
| `Delete` / `Backspace` | Delete selection |
| `Ctrl/Cmd + A` | Select all |
| `Ctrl/Cmd + C / X / V` | Copy / cut / paste |
| `Ctrl/Cmd + Z` / `Ctrl/Cmd + Y` | Undo / redo |
| `Ctrl/Cmd + S` | Save project JSON |
| `Ctrl/Cmd + K` | Command palette |
| `0` / `+` / `-` | Fit / zoom in / zoom out |
| `G` / `O` | Grid / onion skin |

## Notes

- Video export support depends on the browser's `MediaRecorder` codecs. Chrome/Edge are
  the best bet; H.265 is rare.
- Imported raster images are embedded in the project JSON, so large files create large
  projects.
- PSD/AI import is best-effort. For production work, export SVG or PNG from the source
  application first.
