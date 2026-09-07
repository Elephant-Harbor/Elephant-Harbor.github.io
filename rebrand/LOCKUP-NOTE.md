# Header lockup

## Issue
SVG lockup matched `/brand/` markup but `<text font-family="Manrope">` fell back to a serif system face when the file was loaded as `<img>` (browsers do not apply page `@font-face` inside SVG-as-image).

## Current fix (site-rebrand)
- **Header:** HTML lockup — Harbor Gate `mark.svg` + CSS Manrope title-case **Elephant Harbor** (Modern Operator). Guarantees sans wordmark via `tokens.css`.
- **SVG assets:** `lockup.svg` / `lockup-on-ink.svg` outlined from Manrope 700 (no `<text>`), safe for `<img>` / OG reuse.
- **PNG exports:** `lockup-512.png` / `lockup-1024.png` retained (Maren brand export) as optional raster fallback; not used in header.

Hold production cutover until domain email + Thomas greenlight.
