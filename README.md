# Kaiju Kat

A music-reactive arcade visualizer. Cat-eared invaders sit dark until audio
lights them up (mapped across the frequency spectrum), and the whole grid
shakes + cycles color (green → pink → purple → blue) during louder,
climactic moments.

Two audio sources:
- A synthesized mock chiptune (Web Audio API oscillators, no audio files)
- Live microphone input

## Deploying to GitHub Pages
 GitHub URL
   ```
   https://mjin8.github.io/KaijuKat/
   ```
   It can take a minute or two to go live after the first deploy.

## Notes

- The microphone feature requires the page to be served over **HTTPS**
  (GitHub Pages does this by default) — browsers block mic access on
  plain HTTP.
- Everything runs client-side in the browser; there's no server or backend.
