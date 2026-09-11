# Site elevation — `site-elevation`

First-pass elevation of elephantharbor.com. Modern Operator expression on the existing Manrope + Source Serif 4 / Harbor Gate foundation. No new logo.

## Key changes (7)

1. **Positioning locked in public copy** — Hero: “An AI-native operating company.” Sub: find opportunities → build independent businesses → operate what earns the right to continue. Homepage is not an agent-architecture explainer.
2. **IA rename** — Nav is Home · Portfolio · Approach · Contact (Privacy in footer). `/portfolio/` is canonical; `/companies/` and `/ventures/` redirect. `/about/` redirects to `/approach/`.
3. **Homepage completeness** — Seven required sections: hero with abstract signal/horizon visual; signals → businesses; Discover→…→Learn cycle; independent ventures; Setaside portfolio card; operating principles; closing brand statement.
4. **Visual depth** — Sticky translucent header; larger PNG lockup (~1.6×); radial glows, grid, noise, glass cycle cards, card hover, scroll reveals — calm dashboard vocabulary, not neon AI.
5. **Approach page** — Expanded philosophy: originate; evidence over attachment; independent by design; autonomous execution governed where it matters; small experiments; resources follow evidence; learning compounds.
6. **Truthful portfolio** — Setaside Designs only (Etsy; 2026 self-employed bookkeeping spreadsheet). Endorsement line retained. No invented ventures, revenue, customers, testimonials, or team scale.
7. **a11y + performance** — `prefers-reduced-motion` disables glow/pulse/reveal motion; focus rings; semantic HTML; skip link; lightweight `site.js` (no animation framework).

## Positioning decisions

- **AI-native operating company** leads; agentic execution is one sentence under “How we operate,” not the homepage thesis.
- **“Different companies. Further together.”** kept as motto (ventures section + close + footer).
- **Contact remains `elephantharborhq@gmail.com`** — do not claim `hello@` is live.
- Vocabulary: signal / depth / current / horizon — no nautical clichés, no Foundry/Capital/Presence internals on the public site.

## Deliberate rejections

- No new mark or lockup redesign (PNG `assets/lockup-512.png` only for `<img>`).
- No invented portfolio entries or social proof.
- No “What we are / What we are not” lead; no we-believe lists; no innovative/cutting-edge/transformative mush.
- No heavy animation libraries (GSAP, Lottie, etc.).
- No analytics/trackers (CI still greps for them).
- GitHub Pages still deploys **main only** — branch previews are local/static, not a second Pages environment.

## How to preview (branch)

Pages source is `main` → `elephantharbor.com`. To preview this branch before merge:

```bash
cd Elephant-Harbor.github.io
git checkout site-elevation
python3 -m http.server 8080
# open http://localhost:8080/
```

## Second-pass recommendations

1. Custom OG image that matches the elevated hero (current `og.png` still works; refresh for social parity).
2. Domain email cutover when SPF/DKIM/DMARC are ready — then replace Gmail in one pass.
3. Optional second portfolio card layout polish when a second public venture exists (grid already scales).
4. Consider a subtle reduced-data hero SVG asset vs inline if caching/CDN policies change.
5. Lighthouse pass on contrast for muted text on fog sections; tweak `--eh-text-muted` if needed after real-device review.
6. If branch previews become routine, add a workflow that publishes `site-*` to a `*.github.io` preview path (today: main-only by design).
