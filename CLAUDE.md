# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the GitHub Pages marketing/landing site for **SILENTCHAIN AI**, an AI-powered Burp Suite security extension. The site is hosted at https://silentchain.ai via CNAME. This repo contains **only the website** — the actual Burp Suite extension code lives elsewhere.

## Tech Stack

- Pure static HTML/CSS — no build system, no JavaScript frameworks, no dependencies
- Single `index.html` (embedded CSS, ~31KB) serves the entire site
- Fonts: JetBrains Mono (code/monospace), Syne (display headings) via Google Fonts
- Deployed directly via GitHub Pages (no CI/CD pipeline)

## Development

No build, lint, or test commands exist. To develop:

- Edit `index.html` directly
- Preview locally by opening `index.html` in a browser
- Push to `main` branch to deploy via GitHub Pages

## Architecture

The site is a single-page layout in `index.html` with these sections (in order): navigation, hero, stats panel, features grid, code example with terminal simulation, Community vs Professional comparison table, CTA, and footer.

All CSS is embedded in `<style>` tags within `index.html`. The design system uses a dark theme (#0a0e1a background) with cyan (#4de8ff), blue (#0080f0), and green (#00ff88) accents. CSS animations handle grid movement, floating orbs, fade-in-up transitions, and hover effects.

## Key Files

- `index.html` — entire website (markup + styles)
- `CNAME` — custom domain mapping to silentchain.ai
- `README.md` — comprehensive product documentation (installation, configuration for Ollama/OpenAI/Claude/Gemini, usage, troubleshooting)
- `images/` — screenshot assets

## Important Context

- The README documents the Burp Suite extension product, not this website repo
- The project distinguishes Community (free) and Professional editions
- External contributions are not accepted (proprietary, source-visible license)