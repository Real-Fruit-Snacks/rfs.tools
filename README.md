# rfs.tools

The front door at https://rfs.tools: one page, the RFS mark and tagline, a button to [github.com/Real-Fruit-Snacks](https://github.com/Real-Fruit-Snacks). No build step, no framework, nothing loaded from other sites.

| File | Edit when |
|---|---|
| `index.html` | Copy or layout changes. Tokens at the top of `<style>` mirror `rfs-brand/brand/tokens/rfs.css`; change them there first. |
| `fonts/` | IBM Plex woff2 (OFL, `fonts/OFL.txt`). Sans 400/700, Mono 400/600. |
| Icons, `manifest.webmanifest`, `assets/og.png` | Only when `rfs-brand` changes. Copy, don't redraw. |
| `CNAME` | The custom domain GitHub Pages serves. |

Themes: Nightshift (default) / Dayshift. Follows the OS preference, remembers the toggle in `localStorage`.

Hosting: GitHub Pages from `main`, custom domain `rfs.tools`, DNS at Cloudflare (A and AAAA records to GitHub Pages, DNS only so GitHub issues the certificate). The full tool list stays at https://real-fruit-snacks.github.io/.

Brand guide: https://github.com/Real-Fruit-Snacks/rfs-brand/blob/main/BRAND.md
