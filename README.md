# Addressing the Polycrisis

A digital report by H Heuristics on the coupled loops of pollution, global warming, and poverty — and the levers that break them.

**Live site:** deployed via GitHub Pages from the `main` branch (root).

## Structure

- `index.html` — the full single-page report (prose, charts, loop diagram, agenda, sources)
- `assets/chart.umd.min.js` — vendored Chart.js 4.4.1 (no CDN dependency at runtime)
- `draft.md` — the linted prose source (english-report-writing skill, `prose_lint.py` passes with 0 errors)

## Stack

- Static HTML/CSS/JS — no build step
- Chart.js 4 (vendored locally) for figures; inline SVG for the loop diagram
- Typefaces: Newsreader, Source Serif 4, Inter (Google Fonts)
- Light print editorial design

## Deploy

1. Push to `main`.
2. In the GitHub repo: **Settings → Pages → Deploy from branch → `main` / `/ (root)`**.
3. The site publishes at `https://Hunterhghs.github.io/Addressing-the-Polycrisis/`.

## Verification

Pre-push quality gate: `python3 fable-verify.py .` (Veles / Fable-5 verifier) plus `prose_lint.py` for the prose.
