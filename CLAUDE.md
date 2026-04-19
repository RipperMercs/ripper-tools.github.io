# Ripper Tools

## About
Personal landing page for RipperMercs showcasing free tools and personal websites. Single-page static site hosted on GitHub Pages at ripper.tools.

## Structure
- `index.html`: Single-page site with inline CSS and JS (CRT/terminal aesthetic)
- `CNAME`: GitHub Pages custom domain (ripper.tools)

## Sections
1. **Available Tools** [01] to [06]: Mining Hardware Monitor, Background Remover, GIF to MP4, NetGuard, TF-Cleaner, Odds Oracle. Cards link to GitHub repos.
2. **Websites** [01] to [03]: TerminalFeed, TensorFeed, Phreak.fm. Cards link to live domains.
3. About box, Links/Donate row, Footer, Hit counter.

## Design
- Terminal/CRT aesthetic: green-on-dark (`#00ff44` on `#06060a`), Courier New/monospace.
- Scanline sweep, static scanlines, vignette, flicker animation.
- Cards use staggered `fadeSlideIn` animation delays, 0.12s apart.
- Tool cards are clickable, open external link in new tab.

## Adding a new card
1. Copy an existing `<div class="tool-card">` block.
2. Update number, name, tag, status, description, tech, and target link.
3. Set `animation-delay` to previous card's delay + 0.12s.
4. Bump the About box delay to remain after all cards.

## Editing rules
- No em dashes. No double hyphens as substitutes. Use commas, periods, colons, semicolons, or parentheses instead.
- Everything stays inline: no build step, no external dependencies.
- Vary card descriptions naturally, match existing tone (terse, slightly dry, no marketing fluff).

## Deploy
Push to `main`. GitHub Pages rebuilds automatically. Custom domain set via `CNAME`.
