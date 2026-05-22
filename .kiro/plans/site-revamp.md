# Site Revamp Plan: frank-engel.github.io

## Overview

Migrate professional profile site from Bulma/webpack single-page HTML to a Zensical-powered static site with Markdown content, modern theme, and GitHub Pages deployment.

## Requirements

1. Modern look and feel (Zensical `modern` theme variant, teal/amber palette, light/dark toggle)
2. Content updated from DSR (May 2026) -- easy to maintain via Markdown
3. Hidden `#ivy-version` and `#ivy-announcement` divs retained (used by IVyTools app)
4. Deploys as GitHub Pages static site

## Architecture

- **Generator**: Zensical (pip install)
- **Config**: `zensical.toml`
- **Content**: `docs/` directory (Markdown)
- **Overrides**: `overrides/` (footer template for hidden IVy divs)
- **Deploy**: GitHub Actions → GitHub Pages

## Navigation (Tabs)

```
Home | Projects | Publications | CV | About
```

## Color Scheme

- Primary: `teal`
- Accent: `amber`
- Scheme: light/dark toggle

## Content Pages

| Page | Source |
|------|--------|
| `docs/index.md` | Hero landing page |
| `docs/about.md` | Bio, contact, social links |
| `docs/projects/index.md` | Card grid of all projects |
| `docs/projects/ivy-tools.md` | DSR Contribution 1 |
| `docs/projects/nims.md` | DSR Contribution 2 |
| `docs/projects/cameradcp.md` | DSR A5 |
| `docs/projects/surfveltools.md` | DSR Contribution 3 |
| `docs/projects/prob-concept.md` | DSR A3 |
| `docs/projects/echo.md` | DSR A6 (NEW) |
| `docs/projects/river-ice.md` | RIce-Net paper |
| `docs/projects/ml-image-vel.md` | Auto-STIV / AIPIV |
| `docs/projects/training.md` | Training curriculum |
| `docs/publications.md` | Selected pubs from DSR Sec B |
| `docs/cv.md` | Career timeline + PDF link |

## Imagery Needs (TODO for Frank)

- [ ] Updated IVyTools v1.4 screenshot
- [ ] NIMS/HIVIS current map screenshot (1000+ cameras)
- [ ] CameraDCP field deployment photo
- [ ] ECHO AI Skunkworks cover image
- [ ] Auto-STIV / ML project cover images
- [ ] Updated headshot (optional)

## Key Constraints

- The `#ivy-version` and `#ivy-announcement` divs MUST be present in the rendered HTML footer with `display: none` CSS
- Site must deploy from `master` branch push
- Output goes to `site/` directory (Zensical default)
