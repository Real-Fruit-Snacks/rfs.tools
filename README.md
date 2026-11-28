# rfs.tools

Single-page Cyclorama Dawn front door at rfs.tools

Live at **[https://rfs.tools/](https://rfs.tools/)** in the **Cyclorama Dawn — Steel & Beacon Orange** identity. No build step, no frameworks, zero third-party requests.

| File | Purpose |
|---|---|
| `index.html` | Self-contained front door with Cyclorama Dawn tokens, `RFS` stencil wordmark, and interactive 16-channel Signal Patch Bay + 3×6 DMX Cue Matrix |
| `fonts/` | Self-hosted SIL OFL variable WOFF2 files (`Big Shoulders Stencil`, `Albert Sans`, `Azeret Mono`) |
| `icon.svg`, `favicon.ico`, `apple-touch-icon.png`, `icon-*.png`, `manifest.webmanifest` | Copied directly from `rfs-brand/brand/web/` |
| `assets/og.png` | `1280×640` org social preview copied from `rfs-brand/brand/social/rfs-social-org-dark-1280x640.png` |
| `CNAME` | Custom domain (`rfs.tools`) for GitHub Pages |

## Theme & Motion

- Defaults to **Beacon Horizon Dark (`LX 263`, `#050507`)** via `<meta name="color-scheme" content="dark">` with an explicit **Alabaster Day Light (`LX 512`, `#F5F7F9`)** toggle persisted in `localStorage` (`color-scheme`).
- Animations, Beacon proof-beam sweeps, and radial View Transitions are enabled by default; auto-cycling pauses on hover, focus, or the `Pause` control.

Full interactive catalog: **[https://real-fruit-snacks.github.io/](https://real-fruit-snacks.github.io/)**  
Brand system: **[https://github.com/Real-Fruit-Snacks/rfs-brand](https://github.com/Real-Fruit-Snacks/rfs-brand)**
