# Header lockup fidelity

`assets/lockup.svg` matches `/brand/assets/lockup.svg` (Manrope in `font-family`).

When that SVG is used as `<img>`, browsers do **not** apply page `@font-face`, so the wordmark can fall back to a system serif and fail Modern Operator fidelity.

**Fix (pre-cutover):** header uses `assets/lockup-512.png` from `/brand/exports/` (Manrope outlined/baked). Keep SVG for editable source sync with brand; prefer PNG (or outlined SVG) for production `<img>` lockups.
