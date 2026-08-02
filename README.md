# Score Tracker

A mobile-first board game score tracker with a built-in timer. The whole game fits on one screen — no scrolling, at any player count. Plain HTML/CSS/JS, no build step, deployed via GitHub Pages.

Live: https://timvanderwoude.github.io/score-tracker

## Features

- Add/remove players (up to 12), each with a running score and its own accent color
- Score grid auto-fits the screen — cards resize to whatever grid keeps everyone visible without scrolling, in portrait or landscape
- Tap +/− to step a score, press-and-hold to accelerate, or tap the number to open a keypad that can either set it to an exact value or add/subtract any amount
- Up to 6 customizable preset chips per card (any positive or negative value) for games that don't score in single fixed steps (e.g. 2/3-point baskets, cribbage's odd point values, Yahtzee category scores, darts subtracting large amounts) — configurable in Settings, with a few example presets to start from
- Timer with Countdown and Stopwatch modes (start/pause/reset), tucked into a compact drawer so it doesn't eat board space; duration is set microwave-style (type "130" for 1:30) instead of scrolling two pickers
- Multi-level undo/redo covers every destructive action (score changes, add/remove player, reset) — no confirmation dialogs needed
- Turn tracking with a "Next turn" indicator (or auto-advance the turn on every score change, if you'd rather not tap it manually), and an optional leader crown (highest or lowest score wins)
- A History view (Settings → History) logs every score change turn-by-turn, with a break wherever the turn changed — it's kept in sync with undo/redo, so undoing a mistake removes it from the log too
- Settings sheet: score step size, quick-add chips, allow/disallow negative scores, turn tracking, sound, vibration, keep-screen-awake, light/dark/auto theme
- State persists locally (localStorage) — including a running timer, which resumes correctly across a reload (undo history and the History log are session-only, and reset when the page reloads)
- Visual design follows Apple's iOS Human Interface Guidelines (system colors, materials, native control shapes) so it feels like an installed app rather than a web page, especially when added to an iPhone/Android home screen

## Development

Just open `index.html` in a browser — no build step or dependencies.
