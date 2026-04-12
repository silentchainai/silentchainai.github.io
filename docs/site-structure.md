# Site Structure

## Overview

The SILENTCHAIN website is a multi-page static site with no build system or JavaScript frameworks. All pages are mobile-responsive.

## Files

```
silentchainai.github.io/
  index.html            # Landing page (HTML + embedded CSS)
  about.html            # About / team page — mobile-responsive
  enterprise.html       # SILENTCHAIN Enterprise product page — mobile-responsive
  professional.html     # SILENTCHAIN Professional product page — mobile-responsive
  source.html           # SILENTCHAIN SOURCE product page — mobile-responsive
  rag-engine.html       # RAG Knowledge Engine product page — mobile-responsive (untracked, staged)
  privacy.html          # Privacy policy
  terms.html            # Terms of service
  robots.txt            # Allows all crawlers, references sitemap.xml
  sitemap.xml           # 11 URLs (core pages + 3 blog posts)
  CNAME                 # Custom domain: silentchain.ai
  images/               # Screenshot assets and logos
  README.md             # Product documentation (not the website docs)
  CLAUDE.md             # Developer architecture notes
  blog/
    index.html          # Blog listing page — mobile-responsive
    why-rag-changes-everything-for-ai-vulnerability-scanning/
      index.html        # Blog post — mobile-responsive, BlogPosting + Organization + BreadcrumbList JSON-LD
    ai-pentesting-tools-2026-comparison/
      index.html        # Blog post (untracked, staged) — BlogPosting + Organization + BreadcrumbList JSON-LD
    ai-code-security-scanners-2026-codex-semgrep-alternatives/
      index.html        # Blog post (untracked, staged) — BlogPosting + Organization + BreadcrumbList JSON-LD
    rag-for-vulnerability-detection/
      index.html        # Blog post (untracked, staged) — BlogPosting + Organization + BreadcrumbList JSON-LD
    silentchain-vs-burpgpt-vs-burp-ai-agent/
      index.html        # Blog post (untracked, staged) — BlogPosting + Organization + BreadcrumbList JSON-LD
    building-an-attack-chain-engine/
      index.html        # Blog post (untracked, staged) — BlogPosting + Organization + BreadcrumbList JSON-LD
    mcp-server-security-ai-agent-attack-surface/
      index.html        # Blog post (untracked, staged) — flagship MCP security deep-dive (~3,600 words), BlogPosting + Organization + BreadcrumbList JSON-LD
    phase-2-active-verification-false-positives/
      index.html        # Blog post (untracked, staged) — Phase 2 active verification explainer, BlogPosting + Organization + BreadcrumbList JSON-LD
```

## Pages

### `index.html` — Landing Page

Contains these sections in order:

1. **Navigation** — Fixed header with logo and nav links (Products dropdown)
2. **Hero Banner** — Product tagline and CTA button
3. **Stats Panel** — Key metrics (vulnerability types, AI models, etc.)
4. **Features Grid** — Feature cards with descriptions
5. **Code Example** — Terminal simulation showing scanner output
6. **Edition Comparison** — Community vs Professional vs Enterprise vs SOURCE feature table (4 columns, 15 feature rows)
7. **Call to Action** — Download/purchase buttons
8. **Footer** — Links, copyright, social (X, GitHub, YouTube)

### `about.html` — About Page

Company background, mission, and team information. Positioned as "AI-powered product division of Sn1perSecurity LLC."

### `enterprise.html` — Enterprise Edition

Product page for SILENTCHAIN Enterprise: standalone CLI/API, async scanning, SQLite persistence, RAG integration. Differentiates from Community/Pro.

### `professional.html` — Professional Edition

Product page for SILENTCHAIN Professional: Burp Suite extension with Phase 2 active verification, WAF detection, OOB testing, 250+ payloads, 7 AI providers.

### `source.html` — SOURCE Edition

Product page for SILENTCHAIN SOURCE: AI static code vulnerability scanner with 4-phase pipeline, PoC generation, attack chain construction, Docker sandbox. Internal link to MCP blog post from Cross-Product Correlation feature card.

### `rag-engine.html` — RAG Knowledge Engine (untracked, staged)

Dedicated product page for the RAG Security Knowledge Engine: KB sources, correlation rules, feedback loop, API reference, terminal visuals. Not yet committed.

### `blog/index.html` — Blog Listing

Lists published blog posts. Currently staged: 8 posts total. All 8 posts have BlogPosting + Organization + BreadcrumbList JSON-LD structured data.

## SEO / Discoverability

- `robots.txt` — allows all crawlers, references `sitemap.xml`
- `sitemap.xml` — lists 11 URLs: `/`, `/about`, `/enterprise`, `/professional`, `/source`, `/blog/`, 3 blog posts (`mcp-server-security-ai-agent-attack-surface`, `phase-2-active-verification-false-positives`, `why-rag-changes-everything-for-ai-vulnerability-scanning`), `/privacy`, `/terms`
  - **Gap:** sitemap does NOT include `rag-engine.html` or the 5 remaining blog posts (`ai-pentesting-tools-2026-comparison`, `ai-code-security-scanners-2026-codex-semgrep-alternatives`, `rag-for-vulnerability-detection`, `silentchain-vs-burpgpt-vs-burp-ai-agent`, `building-an-attack-chain-engine`) — update before publish
- Structured data: All 8 blog posts have BlogPosting + Organization + BreadcrumbList JSON-LD (added 2026-04-11)
- Meta tags: Open Graph + Twitter Card present on `index.html`, `enterprise.html`, `professional.html`, `source.html`. Missing Twitter Card on `about.html` and `blog/index.html`.

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
