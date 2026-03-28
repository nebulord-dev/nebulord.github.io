# Nebulord Site

Static landing page for [nebulord.dev](https://nebulord.dev) — a suite of developer tools.

## Stack

- Pure HTML + CSS, no build step, no JS
- Deployed via GitHub Pages with custom domain (`CNAME → nebulord.dev`)
- Files: `index.html`, `styles.css`, `CNAME`, plus `images/` (background photo, logo)

## Design

- Dark theme with noise/grid texture overlays and a background photo (`images/bg.jpg`) with blur, sepia, and hue-rotate filters
- Tool cards use a `--accent` CSS custom property set on each card element — tool name color, tag color, tag border, and tag background all derive from `--accent` via CSS (using `color-mix()`). Do not add inline color styles to tags or names.
- Tools 04 (Trialrun) and 05 (Covermap) are marked "Coming soon" with `.nb-soon-badge`
- Hero section uses a flex layout (`.nb-hero-top`) with text left and logo right; stacks vertically on mobile via `@media (max-width: 768px)`
- All classes are prefixed `nb-` to namespace styles

## Editing Notes

- No build/deploy pipeline to run — push to `main` and GitHub Pages picks it up
- Keep it vanilla: no frameworks, no bundlers, no JS unless absolutely necessary
- When adding/editing tool cards, only set `--accent` on the card element — colors cascade from there
