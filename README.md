# Missio.io — bold website redesign (design package)

A complete redesign proposal for missio.io, built as real, responsive HTML/CSS using the content of the current site (missio-qa.missio.io).

**The idea:** Missio's logo is five connected nodes, so the whole site is built on that network: four engines meeting in one supporter record. Giant type and confident colour blocks bring the specialist-agency boldness. Real product UI, real customers, cited sources and an honest comparison bring the trust.

## Open the prototype

| Page | File | Presentation states |
|---|---|---|
| Homepage | `site/home.html` | `#mega` opens the Platform mega-menu · `#menu` opens the mobile menu (at ≤ 760 px) |
| Service page: Growth Engine | `site/growth-engine.html` | — |
| Hero board (entry image 1) | `entries/entry-1.html` | 1600 × 1200 at 1.5× |
| Package board (entry image 2) | `entries/entry-1-detail.html` | 1600 × 7543 |

Clicking “Platform” on the homepage opens the mega-menu (Esc or click-away closes it). The burger opens the mobile menu sheet.

## Design tokens (`site/missio.css`)

- **Colour:** Missio Teal `#02647E` · Deep Mission `#062A33` · Spark Amber `#F2A73D` (actions only) · Warm Paper `#F2EDE4` · Signal Sky `#4FB3CC` · Ink `#16262D`. Engine colours: Growth `#F2A73D`, Relationship `#4FB3CC`, Execution `#E0734F`, Revenue `#2FA58C`.
- **Contrast (WCAG 2.2 AA):** Ink/Paper 13.3:1 · Teal/White 6.7:1 · Ink/Amber 7.7:1 · Paper/Deep Mission 13.0:1 · Sky/Deep Mission 6.2:1.
- **Type:** Bricolage Grotesque 700–800 (display, −3.5 % tracking) + Inter 400–700 (text/UI, tabular figures). Both from Google Fonts. Scale: 104 · 64 · 46 · 28 · 20 · 17 · 12.5 px.
- **Spacing:** 4-pt scale: 4 · 8 · 16 · 24 · 32 · 48 · 64 · 96. **Radius:** 10 · 16 · 24 · 32 · pill. **Elevation:** e1 card · e2 floating UI · e3 modal.

## Grid & breakpoints

| Width | Columns | Margin | Gutter |
|---|---|---|---|
| 1440 | 12 | 80 | 24 |
| 1024 | 12 | 48 | 20 |
| 768 | 8 | 32 | 16 |
| 390 | 4 | 20 | 12 |

## Interaction notes

- **Mega-menu:** opens on click or 150 ms hover-intent. Esc closes it and focus stays trapped inside while open. Every engine is 2 clicks from any page.
- **Service pages:** a sticky sub-nav with “Let's talk” appears after the hero.
- **Mobile:** a sticky “Let's talk” bar, and a one-sheet menu with no nested accordions, so any page is 2 taps. The comparison table collapses to a 2-up “compare with” picker. Tap targets are at least 44 px.
- **Motion:** 200–320 ms ease-out, and `prefers-reduced-motion` is respected.

## Assets

- `assets/missio-logo-{teal,cream,ink}.svg`: the supplied logo, unchanged, in three colourways.
- `assets/missio-mark-{teal,cream,amber}.svg`: the node mark on its own.
- Line icons are inline SVG: 24 px, 1.9 stroke, round joins.
- Photography comes from the current Missio site and is used only as placeholders.

Numbers shown in product UI (gifts, tickets, shifts) are sample data. Stats and claims come from the current Missio site.
