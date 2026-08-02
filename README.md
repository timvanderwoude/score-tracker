# Score Tracker

A mobile-first board game score tracker with a built-in timer. The whole game fits on one screen — no scrolling, at any player count. Plain HTML/CSS/JS, no build step, deployed via GitHub Pages.

Live: https://timvanderwoude.github.io/score-tracker

## Features

- Add/remove players (up to 12), each with a running score and its own accent color
- Score grid auto-fits the screen — cards resize to whatever grid keeps everyone visible without scrolling, in portrait or landscape
- Tap +/− to step a score, press-and-hold to accelerate, or tap the number to type an exact value
- Timer with Countdown and Stopwatch modes (start/pause/reset), tucked into a compact drawer so it doesn't eat board space
- Multi-level undo covers every destructive action (score changes, add/remove player, reset) — no confirmation dialogs needed
- Turn tracking with a "Next turn" indicator, and an optional leader crown (highest or lowest score wins)
- Settings sheet: score step size, allow/disallow negative scores, sound, vibration, keep-screen-awake, light/dark/auto theme
- State persists locally (localStorage) — including a running timer, which resumes correctly across a reload

## Development

Just open `index.html` in a browser — no build step or dependencies.
