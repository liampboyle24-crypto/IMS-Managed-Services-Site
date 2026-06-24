# Asset Slot Map

Each row = one PNG the redesign run expects. Filenames are fixed; don't rename.
All assets live in `references/generated/`.

| # | Filename | Section in `index.html` | Aspect | Recommended px | Usage / treatment |
|---|---|---|---|---|---|
| 01 | `hero.png` | `#top` (Hero) | 21:9 | 3200 × 1372 | Full-bleed right column behind hero card; navy gradient overlay on left for headline legibility. |
| 02 | `problem.png` | `#problem` ("Install Day Is Not the Finish Line") | 4:5 | 1600 × 2000 | Editorial portrait crop, right-aligned next to split section intro. |
| 03 | `reliability.png` | `#reliability` ("Downtime Is Never Just a Screen Problem") | 16:10 | 2400 × 1500 | Subtle full-bleed background behind stat grid; ~14% opacity navy overlay. |
| 04 | `shift.png` | `#shift` ("We Don't Install AV. We Run It.") | 3:2 | 2400 × 1600 | Large left-image / right-text block. Anchors the navy operational pivot. |
| 05 | `failure-points.png` | `#failure-points` | 4:3 | 2000 × 1500 | Inset image to right of the failure-point list. |
| 06 | `touchless.png` | `#how` ("Touchless Means We Move. Not You.") | 3:2 | 2400 × 1600 | Right side of `.loop-panel`; behind the closed-loop SVG with low opacity, OR full image block above the loop. |
| 07 | `growth.png` | `#growth` ("Reliable AV Is a Growth Lever") | 16:10 | 2400 × 1500 | Replaces the existing inline `<svg>` collab illustration. |
| 08 | `pillar_01_service-support.png` | `#architecture` → Pillar 01 | 4:5 | 1200 × 1500 | Top of `.pillar-card` for Service & Support. |
| 09 | `pillar_02_avaas.png` | `#architecture` → Pillar 02 | 4:5 | 1200 × 1500 | Top of `.pillar-card` for AVaaS. |
| 10 | `pillar_03_staff-augmentation.png` | `#architecture` → Pillar 03 | 4:5 | 1200 × 1500 | Top of `.pillar-card` for Staff Augmentation. |
| 11 | `pillar_04_reporting-4sight.png` | `#architecture` → Pillar 04 | 4:5 | 1200 × 1500 | Top of `.pillar-card` for Reporting / 4Sight. |
| 12 | `proof.png` | `#proof` ("Earned the Right to Say This") | 16:9 | 2400 × 1350 | Background band behind the Integrator-of-the-Year proof feature. |
| 13 | `promise.png` | `#promise` ("We Measure Our Success By Yours") | 21:9 | 3200 × 1372 | Full-bleed banner before the contact section. Counterpoint to the hero. |
| 14 | `contact.png` | `#contact` (CTA / Contact) | 16:9 | 2400 × 1350 | Subtle background to the right of the contact form / email. ~18% opacity. |
| T1 | `texture_navy-grain.png` | reusable | 1:1 | 2048 × 2048 | Tiled overlay on navy sections to break up flat fills. Multiply blend, 30% opacity. |
| T2 | `texture_gold-foil.png` | reusable | 1:1 | 2048 × 2048 | Section dividers + outcome card accent. Soft-light blend. |

### Aspect-ratio cheatsheet for image generators

| Aspect | MJ / SDXL ratio | Common pixel pairs |
|---|---|---|
| 21:9 | `--ar 21:9` | 3200×1372, 2520×1080 |
| 16:10 | `--ar 16:10` | 2400×1500, 1920×1200 |
| 16:9 | `--ar 16:9` | 2400×1350, 1920×1080 |
| 3:2 | `--ar 3:2` | 2400×1600, 1800×1200 |
| 4:3 | `--ar 4:3` | 2000×1500, 1600×1200 |
| 4:5 | `--ar 4:5` | 1200×1500, 1600×2000 |
| 1:1 | `--ar 1:1` | 2048×2048 |

### Consistency rules

- **Pillars (08–11) must be generated as one matched set.** Same time of day, same color grade, same lens, same depth-of-field. If one drifts, regenerate all four.
- **Hero (01) and Promise (13) are a pair.** Hero opens, Promise closes. Generate them as bookends — different rooms, same world.
- **No on-camera people in the hero, problem, or promise frames.** Operational humans only appear in `shift.png`, `pillar_01`, `pillar_03`, and `growth.png`, and even there: never face-forward, never centered, always in motion or three-quarter back.
- **No readable text in any frame.** Display panels can be illuminated and abstract, never spelling words.
