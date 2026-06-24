# Asset Slot Map

One row per section of `index.html`. The **Type** column tells the redesign
pass how to source it.

| Type legend | |
|---|---|
| 📷 | Photo (raster PNG in this folder) |
| 🟦 | Vector / inline SVG written into `index.html` |
| ⬛ | Library icon (Lucide, inline SVG) |
| 🌫 | Texture (CSS / SVG filter, no file) |
| — | No asset; section is type-led |

## Sections

| # | Section in `index.html` | Type | Filename or marker | Aspect / size | Treatment |
|---|---|---|---|---|---|
| 01 | `#top` Hero | 📷 | `hero.png` | 21:9 · 3200 × 1372 | Full-bleed right column behind hero card. Navy gradient overlay on left for headline legibility. **Essential.** |
| 02 | `#problem` Install Day Is Not the Finish Line | — | *(none)* | — | Drop the photo. Type-led section with a single small ⬛ icon next to the eyebrow. |
| 03 | `#reliability` Downtime | 🟦 | inline svg: `uptime-stripe` | ~800 × 120 | Replace background photo with a horizontal SVG strip chart showing 30 days of uptime ticks — 28 navy ticks, 2 gold ticks for outages. Lives above the stat grid. |
| 04 | `#shift` We Don't Install AV. We Run It. | 📷 | `shift.png` | 3:2 · 2400 × 1600 | NOC at night, three-quarter back. **Essential second photo.** Pair to the hero. |
| 05 | `#failure-points` Predictable Failures | ⬛ | Lucide: `volume-2`, `monitor`, `wifi`, `plug`, `terminal` | 32 × 32 each | Five small icons, one per failure category (audio, video, network, power, control software), aligned in a tight strip above the list. |
| 06 | `#how` Touchless (closed loop) | 🟦 | existing SVG | — | Keep the existing `.loop-diagram` SVG. Tighten stroke weight + gold accent on the active node. No new asset. |
| 07 | `#growth` Reliable AV Is a Growth Lever | 🟦 | inline svg: `growth-arc` | ~480 × 360 | Replace the inline collab-room SVG with a cleaner abstract motif: an upward arc of three nodes (Decisions → Impressions → Cost) connected by a thin navy line, gold node at the apex. |
| 08–11 | `#architecture` Four Pillars | 🟦 | inline svg: `pillar-icon-{01..04}` | 64 × 64 each | One abstract line motif per pillar — geometric, not photographic. Set of 4 matched icons sharing stroke weight, navy stroke, single gold accent stroke per icon. Sits at the top of each `.pillar-card`. See `PROMPTS.md § Vector` for the exact concept per pillar. |
| 12 | `#proof` Earned the Right to Say This | — | *(none)* | — | Drop the photo. Lean on the typographic feature block (year, name, badge) and a single thin gold rule above the badge. Type carries trust here. |
| 13 | `#promise` We Measure Our Success By Yours | 📷 *(optional)* | `promise.png` | 21:9 · 3200 × 1372 | Bookend to the hero — end-of-day corridor, one-point perspective. Skip if you want to stay strictly at 2 photos. |
| 14 | `#contact` CTA / Contact | — | *(none)* | — | Drop the photo. Use a flat navy field + the `texture-grain` filter; let the email and CTA be the focal point. |

### Reusable surface treatments

| # | Use | Type | Marker | Notes |
|---|---|---|---|---|
| T1 | Subtle grain on navy sections | 🌫 | inline svg: `texture-grain` | `<feTurbulence baseFrequency="0.9" numOctaves="2"/>` over a navy fill, ~14% opacity multiply. No PNG. |
| T2 | Outcome card accent | 🟦 | inline svg: `gold-mark` | Replace the existing `✓` glyph with a small geometric mark drawn in gold. No PNG. |

### Optional bookend photo

If you want symmetry with the hero, generate `promise.png` (row 13). It's
the only optional 📷 slot. Everything else is either essential, vector, or
removed.

---

### Why each removal

- **Problem, Proof, Contact**: type-led sections. A photo competes with the message instead of carrying it.
- **Reliability, Failure points, Pillars, Growth**: data and structure. Diagrams and icons make the claim; photos only decorate around it.
- **Touchless**: already has a strong SVG. Don't double up.
