# Changelog

## [Unreleased]

> Local-only; publish gated on founder approval per `CLAUDE.md`.

### Added
- New product pages: `enterprise.html`, `professional.html`, `source.html`, `about.html` (commit `a2f4e1d`, 2026-04-07)
- RAG Knowledge Engine product page: `rag-engine.html` — KB sources, correlation rules, feedback loop, API reference, terminal visuals (staged 2026-04-09)
- Blog infrastructure: `blog/index.html` + 8 posts (staged through 2026-04-11):
  - `why-rag-changes-everything-for-ai-vulnerability-scanning/`
  - `ai-pentesting-tools-2026-comparison/`
  - `ai-code-security-scanners-2026-codex-semgrep-alternatives/`
  - `rag-for-vulnerability-detection/`
  - `silentchain-vs-burpgpt-vs-burp-ai-agent/`
  - `building-an-attack-chain-engine/`
  - `mcp-server-security-ai-agent-attack-surface/` — flagship MCP security deep-dive (~3,600 words)
  - `phase-2-active-verification-false-positives/` — Phase 2 active verification explainer
- Products dropdown nav menu and Connect footer section (X, GitHub, YouTube) (commit `a2f4e1d`)
- Products section on homepage with RAG Knowledge Engine card (commit `a2f4e1d`)
- `docs/` directory with `site-structure.md`, `deployment.md`, `maintenance.md`, `README.md` (commit `a2f4e1d`)
- Developer architecture notes in `CLAUDE.md` (commit `a2f4e1d`)
- Mobile-responsive nav, scaled headings, overflow fixes across product pages (commit `a2f4e1d`)
- SEO metadata (Open Graph + Twitter Card) on `about.html`, `enterprise.html`, `professional.html`, `source.html`, `blog/index.html`, and first blog post (commit `f96430c`, 2026-04-08)
- `robots.txt` allowing indexing and referencing the sitemap (commit `f96430c`)
- `sitemap.xml` listing 11 URLs: `/`, `/about`, `/enterprise`, `/professional`, `/source`, `/blog/`, 3 blog posts (`mcp-server-security…`, `phase-2-active-verification…`, `why-rag-changes-everything…`), `/privacy`, `/terms` (updated 2026-04-11)
- BreadcrumbList JSON-LD structured data added to all 8 blog posts (2026-04-11)
- Internal link from `source.html` to MCP server security blog post (2026-04-11)

### Changed
- Replaced nav/footer logo with transparent PNG (commit `a2f4e1d`)
- Updated Sn1per dropdown link to `sn1persecurity.com` (Sn1per AI Core) (commit `a2f4e1d`)
- Removed pricing/Early Bird rows from comparison table pending founder approval (commit `a2f4e1d`)

## [1.0.3] - 2026-02-22

### Added
- YouTube demo video CTA on landing page
- Hardened .gitignore to prevent accidental file commits

## [1.0.2] - 2026-02-15

### Added
- Waiting list signup link for early access

## [1.0.1] - 2026-02-10

### Added
- README documentation
- Logo and theme updates
- Privacy policy page
- Terms of service page

### Changed
- Updated color scheme and branding
- Repository cleanup (removed unused assets)

## [1.0.0] - 2026-02-03

### Added
- Initial SILENTCHAIN website launch
- Landing page with product overview
- CNAME configuration for silentchain.ai domain
