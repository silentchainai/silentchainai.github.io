# Deployment

## GitHub Pages

The site is deployed automatically via GitHub Pages on every push to `main`.

### Custom Domain

The `CNAME` file maps the repository to `silentchain.ai`.

**DNS configuration required:**
- `A` record pointing to GitHub Pages IPs
- `CNAME` record for `www.silentchain.ai` pointing to `silentchainai.github.io`

### Deploying Changes

```bash
cd silentchainai.github.io
# Edit index.html
git add index.html
git commit -m "Update site content"
git push origin main
```

Changes are live within 1-2 minutes of pushing.

### Verifying Deployment

```bash
# Check GitHub Pages build status
gh api repos/silentchainai/silentchainai.github.io/pages

# Or visit directly
curl -sI https://silentchain.ai | head -5
```

## Local Preview

Since the site is pure HTML with no build step:

```bash
# Simple HTTP server for local preview
cd silentchainai.github.io
python3 -m http.server 8888
# Visit http://localhost:8888
```
