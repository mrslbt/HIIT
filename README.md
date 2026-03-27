# HIIT Runner — Treadmill Interval Timer

A browser-based interval timer built for treadmill HIIT workouts. Big countdown, speed cues, audio alerts — designed to be readable mid-sprint.

## What is this?

HIIT Runner guides you through a structured treadmill interval workout: warm up, alternating sprint/recovery cycles, and cool down. It tells you what speed to set on the treadmill and counts down each phase for you, so you can focus on running instead of watching the clock.

## Why?

Most interval timer apps are generic stopwatch tools. They don't tell you what speed to run at, and they're hard to read from a treadmill display shelf. HIIT Runner shows a large countdown timer and the current target speed in km/h, with color-coded phases and audio cues you can hear over the machine.

## How It Works

1. **Warm Up** — ease in at a walking/jogging pace (default 6.0 km/h for 2 minutes)
2. **Sprint** — high intensity (default 12.0 km/h for 30 seconds)
3. **Recovery** — active rest (default 7.0 km/h for 1 minute)
4. **Repeat** — sprint and recovery alternate for a set number of cycles (default 6)
5. **Cool Down** — wind down at a low pace (default 5.0 km/h for 3 minutes)

Every speed, duration, and cycle count is configurable in the settings panel.

## Features

- **Large countdown timer** — Bebas Neue font, readable from a distance while running
- **Speed display** — shows the exact km/h to dial in for each phase
- **Audio cues** — distinct synthesized chime patterns for each phase transition, plus a 3-second countdown warning before every switch
- **Color-coded phases** — amber (warm up), red (sprint), blue (recovery), teal (cool down), green (done) with ambient glow effects
- **Progress tracking** — progress bar, phase indicator strip, and "next up" preview pill
- **Configurable everything** — speeds in 0.1 km/h steps, durations in 5-second steps, cycle count
- **Volume control** — adjustable volume with individual test buttons for each sound
- **Screen wake lock** — prevents your phone from sleeping mid-workout
- **Settings persist** — all preferences saved to localStorage
- **Mobile-first** — optimized for phone screens propped on a treadmill shelf
- **Accessibility** — respects `prefers-reduced-motion`

## Usage

No build step. Just open `index.html` in a browser, or host it anywhere that serves static files.

To run locally:

```bash
git clone https://github.com/mrslbt/HIIT.git
cd HIIT
open index.html
```

## Tech

Zero dependencies — a single HTML file with inline CSS and JavaScript.

- Web Audio API for synthesized audio cues
- Wake Lock API to prevent screen sleep
- CSS custom properties for dynamic phase theming
- localStorage for settings persistence

## Built by

Made in Fukuoka.
