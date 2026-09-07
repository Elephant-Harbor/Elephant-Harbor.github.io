# Elephant Harbor — public parent site

**Live (production):** https://elephantharbor.com/ — served from `main` only.  
**Preview branch:** `site-rebrand` — rebrand rebuild for Thomas / Wells review. **Do not merge to `main` or cut over production until blockers below are cleared.**

Canonical brand kit: https://elephantharbor.github.io/brand/  
Copy pack (this branch): `rebrand/CONTENT-ARCHITECTURE.md`, `rebrand/HOMEPAGE-COPY.md`, `rebrand/ABOUT-COPY.md`

## Sitemap (preview)

| Path | Notes |
|------|--------|
| `/` | Homepage |
| `/companies/` | Public portfolio (Setaside Designs) |
| `/about/` | Diligence substance |
| `/contact/` | Gmail until domain mail works |
| `/privacy/` | No analytics |
| `/ventures/` | Redirect → `/companies/` |
| `/approach/` | Redirect → `/#how-we-work` |

Nav: Companies · About · Contact (How We Work is a homepage section, not a separate page.)

## Preview how-to

GitHub Pages workflow deploys **`main` only** (see `.github/workflows/pages.yml`). This branch is not auto-published to elephantharbor.com.

To preview:

1. Check out `site-rebrand` locally and open `index.html` via any static server, e.g. `python3 -m http.server 8080` from the repo root.
2. Or browse files on GitHub: https://github.com/Elephant-Harbor/Elephant-Harbor.github.io/tree/site-rebrand

## Stack / constraints

- Static HTML/CSS on GitHub Pages
- Self-hosted Manrope + Source Serif 4 (no Google Fonts URLs — CI enforces)
- No analytics, no trackers
- Contact: `elephantharborhq@gmail.com` until domain email is verified

## Cutover blockers (before merging to `main`)

1. **Domain email** — `hello@elephantharbor.com` (or chosen address) must work with SPF/DKIM/DMARC before replacing Gmail on the site.
2. **Legal entity name / street address / phone** — do not invent; escalate when ready to publish.
3. **Preview sign-off** — Maren (brand/copy) + Thomas before production cutover.
4. Pages deploy remains `main`-only until explicitly changed.

## Maintainers

- Brand/copy: Maren (Harbor Presence - CEO)
- Tech: Wells (Portfolio - Systems)
- Portfolio accuracy: Hayes (Portfolio - CEO)
