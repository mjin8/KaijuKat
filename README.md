# Kaiju Kat

A music-reactive arcade visualizer. Cat-eared invaders sit dark until audio
lights them up (mapped across the frequency spectrum), and the whole grid
shakes + cycles color (green → pink → purple → blue) during louder,
climactic moments.

Two audio sources:
- A synthesized mock chiptune (Web Audio API oscillators, no audio files)
- Live microphone input

## Deploying to GitHub Pages

1. Create a new GitHub repo (or use an existing one).
2. Add `index.html` to the root of the repo (this file must be named
   exactly `index.html` for GitHub Pages to serve it as the homepage).
3. Commit and push:
   ```
   git add index.html
   git commit -m "Add Kaiju Kat visualizer"
   git push
   ```
4. In the repo on GitHub: **Settings → Pages**.
5. Under "Build and deployment", set **Source** to `Deploy from a branch`.
6. Set **Branch** to `main` (or whichever branch has the file) and folder
   to `/ (root)`. Save.
7. GitHub will give you a URL like:
   `https://<your-username>.github.io/<repo-name>/`
   It can take a minute or two to go live after the first deploy.

That's it — no build step, no dependencies. It's a single self-contained
HTML file (CSS + JS inline), so nothing else needs to be uploaded.

## Notes

- The microphone feature requires the page to be served over **HTTPS**
  (GitHub Pages does this by default) — browsers block mic access on
  plain HTTP.
- Everything runs client-side in the browser; there's no server or backend.
