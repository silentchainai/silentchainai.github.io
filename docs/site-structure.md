# Site Structure

## Overview

The SILENTCHAIN website is a single-page static site with no build system or JavaScript frameworks.

## Files

```
silentchainai.github.io/
  index.html      # Complete site (HTML + embedded CSS, ~34KB)
  CNAME           # Custom domain: silentchain.ai
  images/         # Screenshot assets and logos
  README.md       # Product documentation (not the website docs)
  CLAUDE.md       # Developer architecture notes
```

## Page Sections

The `index.html` page contains these sections in order:

1. **Navigation** — Fixed header with logo and nav links
2. **Hero Banner** — Product tagline and CTA button
3. **Stats Panel** — Key metrics (vulnerability types, AI models, etc.)
4. **Features Grid** — Feature cards with descriptions
5. **Code Example** — Terminal simulation showing scanner output
6. **Edition Comparison** — Community vs Professional feature table
7. **Call to Action** — Download/purchase buttons
8. **Footer** — Links, copyright, social

## Styling

- All CSS is embedded in `index.html` (no external stylesheets)
- Dark theme: `#0a0e1a` background with cyan, blue, green accents
- Fonts: JetBrains Mono (code), Syne (headings) via Google Fonts
- CSS animations: grid movement, floating orbs, fade-in-up, hover effects
- Fully responsive (mobile, tablet, desktop breakpoints)

## Technology

- Pure HTML/CSS — no JavaScript frameworks
- No build step — edit `index.html` directly
- GitHub Pages hosting with custom CNAME
