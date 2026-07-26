# Simon's Claude Training — CCA Study App

A single-file, offline-capable study app for the **Claude Certified Architect — Foundations (CCAR-F)** exam.
Everything runs client-side in the browser: 11 modules, flashcards, per-module quizzes, Week-1 challenge
quizzes, and a 60-item blueprint-weighted mock exam with per-domain diagnostics.

**Live app:** https://simonusa.github.io/simons-claude-training/

## Progress

- **Saved automatically** in the browser's `localStorage` (key `cca-study-progress-v1`) — modules read,
  best quiz scores, challenge scores, mock-exam domain diagnostics and the fast/deep mode. It survives
  reloads, tab closes and restarts, on that device.
- **Export / import** on the Dashboard (*Progress & sync*) moves progress between devices — e.g. iPhone →
  laptop. Export downloads a `cca-progress-<timestamp>.json` file (or copies the JSON to the clipboard);
  Import accepts a pasted blob or an uploaded file, validates it, and replaces local progress.

No backend, no accounts, no tracking — nothing leaves the device unless you export it yourself.

## Files

- `index.html` — the whole app (HTML + CSS + JS + question bank).

## Local use

Open `index.html` in a desktop browser. On iOS, use the hosted URL above — Safari on iOS does not run
local HTML files opened from Files.
