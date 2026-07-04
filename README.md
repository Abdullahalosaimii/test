# Lattice_OS — Network Surveillance Dashboard

A single-page network monitoring dashboard with a retro CRT / radar / terminal
aesthetic. Built as a front-end concept piece — live-feeling telemetry,
a rotating radar sweep centered on the core router, a boot sequence on load,
and a screen-glitch effect that fires when a node goes down.

![status](https://img.shields.io/badge/status-demo-39FF88)
![type](https://img.shields.io/badge/type-frontend%20concept-0C1B15)

## Live demo

Enable **GitHub Pages** on this repo (Settings → Pages → Deploy from branch
`main`, folder `/root`) and it will be live at:

```
git@github.com:Abdullahalosaimii/test.git>/
```

## Features

- **Boot sequence** — a typed terminal intro plays before the dashboard reveals itself
- **Radar sweep** — concentric rings + a rotating beam centered on the core node
- **Live topology map** — 10 simulated nodes (router, switches, firewall, web/db servers, CDN), with animated traffic pulses along each link
- **Bandwidth & latency charts** — hand-drawn SVG line/area charts, no charting library
- **Alert log** — a `tail -f`-style feed that reacts when a node degrades, fails, or recovers
- **Glitch effect** — the whole screen shakes and flashes red for a moment when a node goes down
- **Fully responsive** — sidebar collapses to a top bar on mobile
- **Accessible** — respects `prefers-reduced-motion`, visible focus states on all controls

## Important note

All data in this project is **simulated**. There is no backend, no real network
connection, and no persistence — every metric, node status, and alert is
generated randomly in the browser with plain JavaScript. Refreshing the page
resets everything. This is a design/front-end showcase, not a production
monitoring tool.

## Stack

Plain HTML, CSS, and vanilla JavaScript. No build step, no dependencies —
just open `index.html` in a browser. Fonts (`VT323`, `IBM Plex Mono`) are
pulled from Google Fonts.

## Running locally

```bash
git clone git@github.com:Abdullahalosaimii/test .git.git
cd <repo-name>
open index.html   # or just double-click the file
```

## Credit

Developed and created by **Abdullah AL-osaimi**.

## License

MIT — see [LICENSE](LICENSE).
