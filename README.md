# The Coltrane Circle

An interactive circle of fifths and Coltrane circle. Build chord progressions, watch them draw geometric patterns across the wheel, and explore the songs, moods and astrological lore behind them.

![Screenshot of the Coltrane Circle](assets/screenshot.png)

## Features

- **Western ↔ Coltrane toggle.** The classic circle of fifths with relative minors, or Coltrane's two whole-tone rings with major-third triangles.
- **Progression builder.** Start a progression on the left (or click the wheel). Next-chord suggestions explain *why* each move works: functional harmony, borrowed chords, secondary dominants, tritone substitutions and Coltrane changes.
- **Geometry.** Each chord change draws a colored line across a starry astrolabe. The color comes from the jump distance (fifth, sextile, square, trine, quincunx, opposition), and each color has its own mood.
- **Famous songs.** Your chords are matched against well-known progressions in any key, with the next chord one click away.
- **Astrology reading.** Zodiac signs (Aries = C), element trines (augmented triads), modality squares (diminished 7ths), aspects and figures like the Grand Trine or Yod, all in tooltips and the pattern panel.
- **Randomize & Mandala.** Generate progressions and layer them into geometric figures. Rotate or drift the wheel.
- **Sound.** Web Audio playback of each chord and the whole progression.

## Controls

| Action | Mouse | Keyboard |
| --- | --- | --- |
| Add a chord | Click a wheel slice or a suggestion | — |
| Remove a chord | Click its chip | Backspace (last chord) |
| Play progression | ▶ Play | Space |
| Randomize | ✦ Randomize | R |
| Rotate the wheel | ⟲ / ⟳ | ← / → |

## Running locally

There's no build step. Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Hosting on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**, set *Source* to "Deploy from a branch", then pick `main` and `/ (root)`.
3. The site will be live at `https://<username>.github.io/<repo>/`.

For link previews (Slack, iMessage, etc.), change the `og:image` meta tag in `index.html` to the full URL, e.g. `https://<username>.github.io/<repo>/assets/social-preview.png`. Some sites ignore relative image paths.

## Project structure

```
index.html                 the whole app (HTML, CSS, JS)
assets/favicon.svg         tab icon
assets/screenshot.png      README image
assets/social-preview.png  link-preview image (1200×628)
.nojekyll                  serve files as-is on GitHub Pages
```

## A note on the lore

The astrological correspondences are a symbolic tradition, not science, and other systems map the signs differently. The two-ring view of Coltrane's circle is one common reading of the drawing he gave Yusef Lateef; musicians interpret it in several ways.

## License

[MIT](LICENSE)
