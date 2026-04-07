# Maintenance

## Updating Content

All content is in `index.html`. Edit sections directly:

### Feature Cards

Find the features grid section and modify card content:

```html
<div class="feature-card">
    <h3>Feature Title</h3>
    <p>Feature description text.</p>
</div>
```

### Edition Comparison Table

Update the Community vs Professional comparison table when features change in either edition.

### Stats Panel

Update metrics when significant milestones are reached (vulnerability types covered, AI models supported, etc.).

## Updating Images

Place new screenshots/assets in the `images/` directory. Reference them in `index.html`:

```html
<img src="images/screenshot.png" alt="Description">
```

Optimize images before committing (PNG for screenshots, SVG for logos when possible).

## Styling Changes

All CSS is embedded in the `<style>` block at the top of `index.html`.

Key CSS variables and colors:
- Background: `#0a0e1a`
- Primary accent: cyan/teal
- Secondary accent: blue
- Success/highlight: green
- Text: white/light gray

## Keeping in Sync

When SILENTCHAIN Community or Professional editions add new features:

1. Update the features grid in `index.html`
2. Update the edition comparison table
3. Update screenshots if the UI changed
4. Push to `main` for automatic deployment
