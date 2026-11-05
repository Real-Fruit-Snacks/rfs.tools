# rfs.tools

The front door at https://rfs.tools: one page, the RFS mark and tagline, a button to [github.com/Real-Fruit-Snacks](https://github.com/Real-Fruit-Snacks). No build step, no framework, nothing loaded from other sites.

| File | Edit when |
|---|---|
| `index.html` | Copy or layout changes. The first token block in `<style>` is pasted verbatim from `rfs-brand/brand/tokens/rfs.css`; change it there first, then paste it again. |
| `fonts/` | IBM Plex woff2 (OFL, `fonts/OFL.txt`). Sans 400/700, Mono 400/600. |
| Icons, `manifest.webmanifest`, `assets/og.png` | Only when `rfs-brand` changes. Copy, don't redraw. |
| `CNAME` | The custom domain GitHub Pages serves. |

Themes: Nightshift (default) / Dayshift. Follows the OS preference (in CSS, so it also works without JavaScript), remembers the toggle in `localStorage` under `rfs-theme`.

## The page

The layout is the org social card (`assets/og.png`, from `rfs-brand/tools/make-org-art.py`) made live: the RFS wordmark, its Ember rule, the tagline and the GitHub button on the left; the cover's `pwsh` panel on the right. The rules come from [BRAND.md](https://github.com/Real-Fruit-Snacks/rfs-brand/blob/main/BRAND.md); only what is specific to this page is written down here.

- **The terminal rows are copied from `rfs-brand/brand/org.toml`**, so the page matches its link preview. When a tool is added, renamed or archived there, update the rows in `index.html` too. Columns are padded with spaces (name to 20 characters, language to 6), as `gh` prints them. On phones the language column is hidden.
- **Motion** (all inside `prefers-reduced-motion: no-preference`; the static page is complete without it): the rule under RFS draws in, the command types, the rows print one by one, the cursor blinks twice and then stays still. On a short screen the run waits until the terminal scrolls into view. The dot grid warms to Ember around the pointer in Nightshift only (Dayshift has no glow). The theme switch sweeps the new theme in from the button.
- **Script**: one inline block at the end of `<body>`, about 40 lines: the theme switch, the hold-until-visible, the pointer light. Without JavaScript the theme follows the OS and the switch is hidden.

Hosting: GitHub Pages from `main`, custom domain `rfs.tools`, DNS at Cloudflare (A and AAAA records to GitHub Pages, DNS only so GitHub issues the certificate). The full tool list stays at https://real-fruit-snacks.github.io/.

Brand guide: https://github.com/Real-Fruit-Snacks/rfs-brand/blob/main/BRAND.md
