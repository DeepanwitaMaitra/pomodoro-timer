# Pomodoro Timer — Personal Productivity Tool

A lightweight Pomodoro timer built with HTML, CSS and vanilla JavaScript.

## Features
- Configurable work and break durations
- Start, pause and reset controls
- Automatic work/break transitions
- Completed-session tracking
- `localStorage` persistence
- Responsive interface

## Tech Stack
HTML5, CSS3, Vanilla JavaScript, browser APIs (`setInterval`, `localStorage`).

## Architecture
User -> HTML/CSS UI -> JavaScript timer/state -> DOM
                                  |
                                  -> localStorage

## Run locally
Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000

## Interview summary
I built a lightweight productivity tool implementing the Pomodoro workflow. JavaScript manages timer state, user events and dynamic DOM updates. `setInterval()` drives the countdown, while `localStorage` persists settings and completed-session count across refreshes.

## Honest scope
This version is frontend-only. It has no authentication, backend API or cloud database. DevOps technologies should only be claimed if they are actually deployed.
