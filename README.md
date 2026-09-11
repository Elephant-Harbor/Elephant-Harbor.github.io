# Elephant Harbor — public parent site

**Live (production):** https://elephantharbor.com/ — served from `main` only (CNAME).  
**Elevation branch:** `site-elevation` — first-pass Modern Operator elevation. See `rebrand/ELEVATION-NOTES.md`.

Canonical brand kit: https://elephantharbor.github.io/brand/

## Sitemap

| Path | Notes |
|------|--------|
| `/` | Homepage — positioning, cycle, portfolio teaser, principles |
| `/portfolio/` | Public portfolio (Setaside Designs) |
| `/approach/` | Philosophy / how we work |
| `/contact/` | Gmail until domain mail works |
| `/privacy/` | No analytics |
| `/companies/`, `/ventures/` | Redirect → `/portfolio/` |
| `/about/` | Redirect → `/approach/` |

Nav: **Home · Portfolio · Approach · Contact** (Privacy in footer).

## Preview how-to

GitHub Pages workflow deploys **`main` only** (see `.github/workflows/pages.yml`). Feature branches are not auto-published to elephantharbor.com.

```bash
python3 -m http.server 8080
# open http://localhost:8080/
```

Or browse on GitHub: https://github.com/Elephant-Harbor/Elephant-Harbor.github.io/tree/site-elevation

## Stack / constraints

- Static HTML/CSS (+ small `site.js`) on GitHub Pages
- Self-hosted Manrope + Source Serif 4 (no Google Fonts URLs — CI enforces)
- No analytics, no trackers
- Contact: `elephantharborhq@gmail.com` until domain email is verified
- Header lockup: PNG only (`assets/lockup-512.png`)

## Maintainers

- Brand/copy: Maren (Harbor Presence - CEO)
- Tech: Wells (Portfolio - Systems)
- Portfolio accuracy: Hayes (Portfolio - CEO)
