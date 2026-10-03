# Classic Solitaire for PewPlay

This directory contains the game adapted for the PewPlay game template. Open `index.html` to play.

`game.json` holds the game page text. `preview.png` and `cover.png` provide the page images. The PewPlay workflow checks pushes to `preview` and `main`.

Game controls: drag cards (mouse or touch, Pointer Events) or tap a card to auto-move it; tap the stock to deal or recycle; Undo, Pause and New game buttons in the top bar (keys: Ctrl+Z/U, P, N, Space).

## Update (October 2026)
- Rewrote the game as a single self-contained `index.html`: no Bootstrap (deleted `bootstrap.min.css`), no external fonts or images (cards, suits and felt are CSS/inline SVG).
- Responsive layout that fills the window: classic layout in portrait and on desktop, side layout (stock left, foundations right) on wide/short screens such as phones in landscape; the tableau fan compresses to fit.
- Drag and drop with mouse and touch, tap-to-move, undo, pause overlay, in-page "New game?" confirmation, Auto Finish, win screen with confetti.
- Saves the game in progress and stats in `localStorage` (`solitario:game`, `solitario:stats`). The original version stored nothing, so no migration was needed.
- New cover and screenshots.
