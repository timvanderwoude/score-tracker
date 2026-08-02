# Score Tracker

A mobile-first board game score tracker with a built-in timer. The whole game fits on one screen — no scrolling, at any player count. Plain HTML/CSS/JS, no build step, deployed via GitHub Pages.

Live: https://timvanderwoude.github.io/score-tracker

## Features

- Add/remove players (up to 12), each with a running score and its own accent color
- Score grid auto-fits the screen — cards resize to whatever grid keeps everyone visible without scrolling, in portrait or landscape
- Tap +/− to step a score, press-and-hold to accelerate, or tap the number to type an exact value
- Up to 6 customizable preset chips per card (any positive or negative value) for games that don't score in single fixed steps (e.g. 2/3-point baskets, cribbage's odd point values, Yahtzee category scores, darts subtracting large amounts) — configurable in Settings, with a few example presets to start from
- A calculator on every card for the amounts your presets don't cover: pick + or −, key in any number, and it's added to or subtracted from the current score in one step
- Timer with Countdown and Stopwatch modes (start/pause/reset), tucked into a compact drawer so it doesn't eat board space; duration is set microwave-style (type "130" for 1:30) instead of scrolling two pickers
- Multi-level undo/redo covers every destructive action (score changes, add/remove player, reset) — no confirmation dialogs needed
- Turn tracking with a "Next turn" indicator, and an optional leader crown (highest or lowest score wins)
- Settings sheet: score step size, quick-add chips, allow/disallow negative scores, sound, vibration, keep-screen-awake, light/dark/auto theme
- State persists locally (localStorage) — including a running timer, which resumes correctly across a reload
- Visual design follows Apple's iOS Human Interface Guidelines (system colors, materials, native control shapes) so it feels like an installed app rather than a web page, especially when added to an iPhone/Android home screen

## Development

Just open `index.html` in a browser — no build step or dependencies.
