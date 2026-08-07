# Pitch View

**Pick your seat at M. Chinnaswamy Stadium — before the first ball is bowled.**

Pitch View is an interactive 3D cricket stadium experience built around TATA IPL 2026, RCB vs CSK at M. Chinnaswamy Stadium, Bengaluru. Fly through the stands, click any seat, and see the exact view from where you'd be sitting.

> **Note:** This is a personal portfolio project. The fixture, pricing, seat availability, and checkout flow are all simulated — no real tickets are sold here.

---

## Features

- Fully procedural 3D stadium — no imported models, all geometry is generated in code
- ~30,000 individually selectable seats rendered with GPU instancing
- RCB batsmen and CSK fielders on the pitch, with live ball physics and a six hit every 8 seconds
- Real crowd audio: ambient stadium loop layered with an IPL roar on every six
- Team-coloured crowd (70% RCB red/black, 30% CSK yellow)
- Solar panel canopy and background parkland matching the real Chinnaswamy skyline
- Animated scoreboard, LED boundary ribbon, floodlight pylons, and sponsor stands
- Named sponsor stands (JioCinema, boAt, BKT, PUMA, Sunrisers, Nothing...) with section colours
- Mini-map, first-person seat view, orbit controls, and keyboard navigation
- Self-contained `index.html` — Three.js + GSAP, no framework

## Run locally

```bash
cd pitch-view
npm install
npm run dev
```

Open the URL shown by Vite (default: `http://localhost:5173`).

## Controls

| Action | Input |
|---|---|
| Orbit the stadium | Click / touch + drag |
| Zoom | Scroll wheel or + / − buttons |
| Select a seat | Click any seat |
| Look around from your seat | Drag while in seat view |
| Exit seat view | Esc or “Back to stadium” |
| Confirm selection | Enter or “Grab seat” |

## Tech

| Library | Purpose |
|---|---|
| [Three.js r128](https://threejs.org/) | 3D rendering |
| [GSAP 3.12.5](https://gsap.com/) | Camera animation |
| [Vite](https://vitejs.dev/) | Dev server / build |

Third-party license details: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)

## Inspiration

Built on top of [StadiView](https://github.com/thebuggeddev/stadiview) by [@thebuggeddev](https://github.com/thebuggeddev) — a beautifully engineered procedural 3D football stadium. The core rendering engine, instanced seat geometry, and camera system all come from that project. This fork converts it into a cricket experience: Chinnaswamy bowl geometry, named IPL sponsor stands, cricket field and players, six animation, and RCB/CSK theming throughout.

## License

This project is a noncommercial adaptation of StadiView, used under the [PolyForm Noncommercial License 1.0.0](LICENSE.md). Original copyright © 2026 thebuggeddev. Modifications © 2026 misal.ships.
