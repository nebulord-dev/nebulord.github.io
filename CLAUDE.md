# Nebulord Site

Static landing page for [nebulord.dev](https://nebulord.dev) — a suite of developer tools.

## Stack

- Pure HTML + CSS, no build step, no JS
- Deployed via GitHub Pages with custom domain (`CNAME → nebulord.dev`)
- Three files: `index.html`, `styles.css`, `CNAME`

## Design

- Dark theme with noise/grid texture overlays
- Tool cards use per-tool accent colors via CSS custom property `--accent`
- Tools 04 (Trialrun) and 05 (Covermap) are marked "Coming soon" with `.nb-tool-card--soon`
- All classes are prefixed `nb-` to namespace styles

## Editing Notes

- No build/deploy pipeline to run — push to `main` and GitHub Pages picks it up
- Keep it vanilla: no frameworks, no bundlers, no JS unless absolutely necessary
- When adding/editing tool cards, follow the existing card markup pattern and accent color convention
