# KONSTRUKTOR

Generative Proun / Mondrian compositions in the browser.

**Live:** [randompatterngeneratorv1.netlify.app](https://randompatterngeneratorv1.netlify.app)

## What it is

A seeded, deterministic pattern generator inspired by El Lissitzky's Proun
plates and Mondrian's grid compositions. Every plate is reproducible from
its seed — same seed and density always produce the same construction.

Two generation modes:

- **Proun** — circle-slice compositions, diagonal wedge beams, thin
  construction lines with marker dots, in the spirit of Lissitzky's Proun
  series.
- **Mondrian** — recursive rectilinear grid subdivision, biased toward
  splitting larger cells first for an asymmetric De Stijl composition,
  thick black grid lines, sparse primary-color fills.

## Controls

- **Style** — switch between Proun and Mondrian generation
- **Seed** — set directly, or click Generate for a random one
- **Density** — controls shape/line/cell count
- **Palette** — four variants per style (classic, steel, olive, mono)
- **Auto-generate** — cycles through new plates on a timer
- **Save SVG / Save PNG** — export the current plate

## Tech

Single-file HTML/CSS/JS, no build step, no dependencies. Deterministic
output via a seeded PRNG (mulberry32). Deploys straight from this repo —
no build command needed, publish directory is the repo root
(`netlify.toml` included).

## Changelog

See the comment block at the top of `index.html` for the full version
history. Bump `APP_VERSION` in the script and add a line there with each
change, same convention used across the other tools in this ecosystem.

---
Joe.K · [axisbim.io](https://axisbim.io)
