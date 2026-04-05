## 2026-04-04 22:13 — Hero section layout redesign: CTA moved inline with headline

**Changes made:**
- `index.html` — Restructured hero into a two-column flex layout (`.hero-split`): headline+tag on the left, CTA button on the right. Added responsive collapse to vertical stack on mobile (≤640px).
- `index.html` — Removed `hero-subtitle` paragraph ("El 78% de los compradores elige al primero que responde…") as it duplicated the proof stats already shown below the fold.

**Decisions:**
- Remove subtitle, not the proof stats — the subtitle repeated the 78% and <2min figures in prose form; the proof stats present them more impactfully as big numbers. Keeping stats, cutting prose.
- CTA floats to the right of the headline rather than below it — creates immediate visual pairing between the problem statement and the call to action.

**Notes:**
Deployed to GitHub Pages via `EdgarTradea/nodograu-com` (main branch). Site lives at nodograu.com.

---
