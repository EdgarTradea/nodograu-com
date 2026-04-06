## 2026-04-06 11:25 — Automatizacion page promoted to homepage, favicon fix, CTA anchor bug

**Changes made:**
- `automatizacion/index.html` — Added missing `id="cta-final"` to the CTA section; all CTAs were pointing to `#cta-final` but the section only had a class, not an id, so clicks did nothing.
- `index.html` — Replaced old homepage with the automatizacion page content. Updated asset paths from `../logo.svg` to `logo.svg`. nodograu.com now shows the automatizacion page directly.
- `favicon.ico`, `favicon-16x16.png`, `favicon-32x32.png`, `apple-touch-icon.png`, `android-chrome-192x192.png`, `android-chrome-512x512.png`, `site.webmanifest` — Added full favicon stack from favicon_io. Previously only an SVG favicon was used, which many platforms render poorly or ignore when generating link previews.
- `index.html` + `automatizacion/index.html` — Added Open Graph meta tags (`og:image` pointing to the 512x512 PNG, `og:title`, `og:description`) so link previews on WhatsApp, iMessage, etc. look correct.

**Decisions:**
- Promote automatizacion page to root — the old homepage was redundant; the automatizacion page is the actual product offering.
- No client dashboard / CRM built — discussed the idea but Edgar has no active clients yet. Decision: use Notion per-client when the first project arrives; revisit building something custom at 3-4 clients if Notion feels limited.

---

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
