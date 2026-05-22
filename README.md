# frank-engel.github.io

Professional profile site for Frank L. Engel, Ph.D. — USGS Geographer and Hydrologic Remote Sensing Scientist.

**Live site:** https://frank-engel.github.io/

## Setup

Built with [Zensical](https://zensical.org/) — a modern static site generator.

### Prerequisites

- Python 3.x

### Local Development

```bash
python -m venv .venv
.venv\Scripts\activate       # Windows
# source .venv/bin/activate  # macOS/Linux
pip install zensical
```

### Preview

```bash
zensical serve
```

Open http://localhost:8000 in your browser.

### Build

```bash
zensical build --clean
```

Output goes to `site/`.

## Deployment

Automatically deployed to GitHub Pages via GitHub Actions on push to `master`. See `.github/workflows/docs.yml`.

## Structure

```
docs/               # Markdown content
  index.md          # Landing page
  about.md          # Bio and contact
  cv.md             # Curriculum vitae
  publications.md   # Selected publications
  projects/         # Individual project pages
  img/              # Images
  stylesheets/      # Custom CSS
overrides/          # Zensical template overrides
zensical.toml       # Site configuration
```

## Note

The `#ivy-version` and `#ivy-announcement` hidden divs in the footer are used by the IVy Tools application for version checking and user notifications. Do not remove them.
