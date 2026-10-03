# Interview Notes

## 30-second explanation
I built a lightweight Pomodoro productivity tool using HTML, CSS and vanilla JavaScript. Users can configure work and break durations, start/pause/reset the countdown, and track completed work sessions. I used `setInterval()` for the countdown and `localStorage` for small persistent settings and session count.

## Key concepts
- DOM manipulation
- Event listeners
- JavaScript application state
- `setInterval()`
- `localStorage`
- Responsive CSS

## Common questions

**What happens when Start is clicked?**
The click event calls `startTimer()`. It creates a one-second interval if a timer is not already running.

**How do you prevent multiple timers?**
`intervalId` is checked before creating an interval.

**What happens at zero?**
The current interval is stopped, the mode changes from work to break or break to work, and the next duration is loaded.

**Why localStorage?**
It provides simple client-side persistence for small non-sensitive values without requiring a backend.

**Why no backend?**
The core functionality is entirely client-side, so a backend is unnecessary for this scope.

**What would you improve?**
I could add browser notifications, statistics, user accounts and cloud synchronization.

**Is this a microservices project?**
No. It is a frontend-only application.

**Can I call it a DevOps project?**
Only if DevOps tooling such as Docker/CI/CD/cloud deployment is actually implemented. This repository does not claim those features by itself.
