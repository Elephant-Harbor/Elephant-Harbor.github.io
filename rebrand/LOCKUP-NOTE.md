# Header lockup

## Issue
SVG `<text font-family="Manrope">` fell back to a serif system face when loaded as `<img>` (page `@font-face` does not apply inside SVG-as-image).

## Current fix (site-rebrand)
- **Header:** brand-export raster `lockup-512.png` (Manrope title-case Modern Operator, Harbor Gate mark).
- **SVG source:** `lockup.svg` / `lockup-on-ink.svg` outlined from Manrope 700 (no `<text>`) for editable/vector use.
- **Larger export:** `lockup-1024.png` available.

Hold production cutover until domain email + Thomas greenlight.
