---
name: IMS Managed Services Platform
description: Reliable collaboration starts before the meeting does.
colors:
  navy-deep: "#002D56"
  navy-night: "#001830"
  ink: "#0A1F3D"
  signal-teal: "#0A6EA8"
  signal-teal-bright: "#71C9F2"
  precision-gold: "#ECAE3D"
  precision-gold-soft: "#F5CB7A"
  ink-on-gold: "#1A1A1A"
  slate: "#4D5D6E"
  muted-steel: "#5B6B7D"
  instrument-mist: "#EEF1F4"
  instrument-mist-deep: "#E2E7EB"
  paper: "#FFFFFF"
  hairline-on-light: "#0A1F3D29"
  hairline-on-dark: "#EEF1F42E"
typography:
  display:
    fontFamily: "Archivo, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Arial, Helvetica, sans-serif"
    fontSize: "clamp(2.625rem, 7.2vw, 6rem)"
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Archivo, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Arial, Helvetica, sans-serif"
    fontSize: "clamp(2.25rem, 5.2vw, 4.5rem)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  subhead:
    fontFamily: "Archivo, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Arial, Helvetica, sans-serif"
    fontSize: "clamp(1.3125rem, 2.25vw, 1.9375rem)"
    fontWeight: 400
    lineHeight: 1.34
  body:
    fontFamily: "Archivo, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, Helvetica, sans-serif"
    fontSize: "clamp(1rem, 1.1vw, 1.125rem)"
    fontWeight: 400
    lineHeight: 1.75
  label:
    fontFamily: "Archivo, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Arial, Helvetica, sans-serif"
    fontSize: "13px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.1em"
rounded:
  hairline: "2px"
  structural: "3px"
  tile: "12px"
  tile-lg: "16px"
  pill: "999px"
  circle: "50%"
spacing:
  margin-mobile: "16px"
  margin-tight: "18px"
  gutter: "24px"
  section-pad: "clamp(88px, 11vw, 158px)"
  container-max: "1180px"
  container-wide-max: "1280px"
components:
  button-primary:
    backgroundColor: "{colors.navy-deep}"
    textColor: "{colors.instrument-mist}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "15px 22px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.navy-deep}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "15px 22px"
  nav-cta:
    backgroundColor: "{colors.navy-deep}"
    textColor: "{colors.instrument-mist}"
    rounded: "{rounded.pill}"
    padding: "10px 14px"
  nav-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "9px 11px"
  card-surface:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.structural}"
  card-surface-navy:
    backgroundColor: "{colors.navy-deep}"
    textColor: "{colors.instrument-mist}"
    rounded: "{rounded.structural}"
---

# Design System: IMS Managed Services Platform

## 1. Overview

**Creative North Star: "The Operator's Blueprint"**

PRODUCT.md states the core positioning in three words: "Operator, not vendor." This system takes that literally rather than figuratively. The page is built like a piece of operational equipment, not a brochure: a faint schematic grid sits under every navy section (`.section--navy::before`, a 64px line grid at 7% opacity), structural panels close to square (2–3px radius) rather than softly rounded, a single typeface carries every register from hero display down to technical micro-labels, and the one recurring decorative motif — concentric pulse rings — is a literal monitoring signal, not an abstract flourish. Nothing about the page is trying to look like a "tech startup." It is trying to look like the inside of a well-run network operations center: precise, calm, and built for people who already know what they're looking at.

The voice is vigilant rather than enthusiastic. Color is committed, not restrained-by-default — navy carries most of the page, Signal Teal carries everyday interactivity and live-state feedback, and Precision Gold is spent on almost nothing, which is exactly why it reads as valuable when it appears. Typography never switches families to manufacture "editorial" contrast; it switches weight, size, tracking, and case instead, the way a technical document would.

This system explicitly rejects the things PRODUCT.md and CLAUDE.md name as anti-references: generic AI-generated visuals, gradient-and-glassmorphism-as-default, fake metrics or unsupported claims, bloated dependencies, and trend-chasing decoration that will date the page in a year. It is not a SaaS landing page wearing a navy suit — it has no hero-metric-card template repeated past the point of meaning, no tiny uppercase eyebrow over every section, and no numbered 01/02/03 scaffolding on cards that aren't actually a sequence.

**Key Characteristics:**
- A single typeface (Archivo) plays every role — display, body, and mono-style technical label — through weight and tracking alone.
- Color strategy is **Committed**: Deep Navy is the dominant surface and text color across the page, not a 10%-restrained accent.
- Precision Gold is the rarest color on the page by design — spent on single moments of proof, never on chrome.
- Depth comes from soft, large-blur ambient shadows and a one-pixel top highlight, not hard drop shadows.
- The only repeating decorative device is the signal/pulse ring — and it always means "this is live," never "this is decoration."
- Shape is tiered by function: sharp for structure, full pill for action, soft tile for icons, true circle for status.

## 2. Colors: The Instrument Panel

The palette reads as an operations console: a deep, near-black navy field, a cool instrument-gray background (not a warm cream — measured at oklch(96% 0.005 248), essentially hueless), one workhorse signal color, and one color spent so rarely it still feels valuable on the fifth scroll.

### Primary
- **Deep Navy** (`#002D56`): The dominant surface and ink color of the entire system — full-bleed section backgrounds, the primary button fill, the nav CTA, and the default heading/body text color on light sections. This is not an accent; it is the page's base register.
- **Navy Night** (`#001830`): The gradient floor under Deep Navy on dark sections (`linear-gradient(165deg, navy-deep, navy-night 78%)`) and the hero photo's scrim. Used to deepen, never used standalone as a flat fill.

### Secondary
- **Signal Teal** (`#0A6EA8`): The everyday interactive and "live" color — link hover states, eyebrow labels, headline accents, stat figures, and the pulse-ring glow that marks the operating-loop diagram as actively monitoring something.
- **Bright Signal** (`#71C9F2`): Signal Teal's on-navy counterpart — used wherever the same role (accent text, stat figures, list markers) sits on a dark background and needs to hold contrast.

### Tertiary
- **Precision Gold** (`#ECAE3D`): Reserved for the single highest-value proof point in a section — a hero stat figure, one status-dot glow, a hover tint on the pillar cards. It is never a body accent, a link color, or a repeated chrome element.
- **Soft Gold** (`#F5CB7A`): Precision Gold's on-navy counterpart, used only where Gold itself would lose contrast against Deep Navy.
- **Ink on Gold** (`#1A1A1A`): The only text color ever placed directly on a gold fill.

### Neutral
- **Ink** (`#0A1F3D`): Default body/heading text on light sections — deliberately darker and slightly more saturated than pure Deep Navy so long-form copy reads with more weight than UI chrome.
- **Slate** (`#4D5D6E`) / **Muted Steel** (`#5B6B7D`): Secondary text and label color on light backgrounds — body copy at reduced emphasis, eyebrow/meta labels.
- **Instrument Mist** (`#EEF1F4`): The page background and on-navy text color. Measured chroma is 0.005 — functionally neutral with a whisper of cool blue, not the warm sand/cream that has become the generic AI default.
- **Mist, Deeper** (`#E2E7EB`): A one-step-darker tint of Instrument Mist for subtle section banding.
- **Paper** (`#FFFFFF`): Card and surface white, used where a light element needs to sit above the Instrument Mist background.
- **Hairline on Light / Hairline on Dark** (`#0A1F3D` and `#EEF1F4`, each at low alpha): The entire border and divider system. There is no solid gray border anywhere in the system — every rule, divider, and outline is a translucent tint of Ink or Mist.

### Named Rules
**The Rare Gold Rule.** Precision Gold is budgeted, not decorative — it appears at most once or twice per section, always on a number or a status signal, never on UI chrome, links, or body accents. If Gold starts showing up more than once per screen, it has stopped being precision.

**The Tinted Hairline Rule.** Borders and dividers are never a flat gray. Every line on the page is a low-alpha tint of Ink (on light surfaces) or Instrument Mist (on dark surfaces) — `hairline-on-light` / `hairline-on-dark`. A solid `#CCCCCC`-style border is a regression, not a simplification.

## 3. Typography: One Voice, Many Registers

**Display / Body / Label Font:** Archivo (with `ui-sans-serif, system-ui, -apple-system, Segoe UI, Arial, Helvetica` fallback)

**Character:** A single geometric grotesque carries the entire page. The CSS exposes `--font-serif`, `--font-sans`, and `--font-mono` as three custom properties, but all three resolve to Archivo — they are role aliases for where a property is conceptually "the editorial voice" or "the technical voice," not a signal to load a second typeface. Register comes entirely from weight (400 body, 700–900 emphasis), tracking (tight negative on display, wide positive on labels), and case (uppercase for labels only).

### Hierarchy
- **Display** (800, `clamp(42px, 7.2vw, 96px)`, line-height 0.92, tracking -0.03em): The hero headline only. `text-wrap: balance` keeps it from breaking awkwardly at narrow widths.
- **Headline** (800, `clamp(36px, 5.2vw, 72px)`): Section-opening headlines (`.headline--section`), max-width 920px so they wrap with intent rather than running the full container.
- **Subhead** (400, `clamp(21px, 2.25vw, 31px)`, line-height 1.34): The secondary line under a section headline — the system's "editorial voice" role, still rendered in Archivo, not a serif.
- **Body** (400, `clamp(16px, 1.1vw, 18px)`, line-height 1.75): Running copy, capped at a 780px measure (roughly 75ch at the largest size).
- **Label** (700, 11–13px, tracking 0.06–0.12em, uppercase): Eyebrows, nav labels, mono-styled meta text (step numbers, credential strip, stat captions). This is the system's "technical voice" — small, wide-tracked, always uppercase, never used for anything a reader needs to linger on.

### Named Rules
**The One Family Rule.** Every register — display, body, and the mono-styled technical label — renders in Archivo. The system never reaches for a second typeface to manufacture "editorial" contrast; it changes weight, size, tracking, and case instead. A pull request that adds a serif or a monospace font file is solving a problem this system already solved without one.

**The Negative-Three Floor.** No heading exceeds -0.03em letter-spacing. Tighter than that and large type starts touching itself instead of reading as "designed."

## 4. Elevation: Ambient Lift and Live Signal

The system is flat by default and lifts only in two specific ways: a soft, ambient shadow for structural surfaces, and a concentric glow reserved exclusively for live-status motifs. There is no hard, dark, tight drop shadow anywhere in the system.

### Shadow Vocabulary
- **Ambient** (`box-shadow: 0 24px 80px rgba(7, 27, 52, .12)`): The default resting elevation for light-surface cards — large blur, very low opacity, no visible offset edge.
- **Card** (`box-shadow: 0 18px 50px rgba(7, 27, 52, .24)`): A more present version of Ambient for surfaces that need clearer separation from a busier background (stat panels, the proof cards).
- **Sheen** (`inset 0 1px 0 rgba(255, 255, 255, .7–.92)`): A one-pixel inset top highlight on light circular and panel elements, simulating a single light source from above rather than a painted gradient.
- **Signal Glow** (e.g. `0 0 0 8px rgba(113, 201, 242, .20), 0 0 32px rgba(10, 110, 168, .50)` for teal; `0 0 0 4px rgba(236, 174, 61, .18)` for gold): Concentric ring glow used exclusively on the operating-loop pulse diagram and status dots. This is the one place the system uses a "glow" — and it is reserved for things that are actually meant to read as live and monitored, never as generic button hover decoration.
- **Grain** (`filter: url(#texture-grain)` at `mix-blend-mode: multiply` over `.section--navy`): A subtle film-grain texture on dark sections — depth through texture rather than through a gradient overlay.

A small number of components (the hero card, the sticky nav once scrolled) additionally use `backdrop-filter: blur()`. Treat that set as closed, not as precedent — see Don'ts.

### Named Rules
**The Ambient-Not-Hard Rule.** Elevation reads through large-blur, low-opacity shadows and a one-pixel top sheen — never a tight, dark, high-opacity drop shadow. If a shadow has a visible hard edge, it's wrong for this system.

**The Signal-Glow Exception.** Concentric ring glows in Signal Teal or Precision Gold mean one thing only: "this is being monitored right now." They belong on the pulse diagram and status dots, not on cards, buttons, or hover states that have nothing to do with live status.

## 5. Components

### Buttons
- **Shape:** Full pill (999px radius), 52px minimum height — never the structural 2–3px radius used on panels.
- **Primary:** Deep Navy fill, Instrument Mist text, Ambient-family shadow (`0 14px 36px rgba(7, 27, 52, .22)`, deepening on hover) — this is the button that should always resolve to the page's single conversion point, `#contact`.
- **Ghost:** Transparent/translucent fill, Hairline border, Deep Navy text on light sections (swapping to Instrument Mist text + Hairline-on-dark border on navy sections). Used for the secondary, exploratory action (e.g. "See the model"), never for the primary conversion action.
- **Hover / Focus:** `translateY(-2px)` lift plus a deepened Ambient shadow; `:active` settles to `translateY(-1px) scale(.97)`. No color-shift-only hover states.

### Cards / Containers
- **Corner Style:** Structural radius (3px) — close to square, "drafting precision," not the soft 8–16px radius common to generic SaaS cards.
- **Background:** Paper on light sections; Deep Navy (gradient to Navy Night) on dark sections.
- **Shadow Strategy:** Ambient or Card from the Elevation vocabulary above; never a hard drop shadow.
- **Border:** Hairline-on-light or Hairline-on-dark only — never a flat gray stroke.
- **Icon tiles inside cards** break the structural radius deliberately: 12px (desktop) to 16px (narrow viewports) on a 48–52px square — a third, distinct "soft squircle" shape reserved only for icon containment, never reused for the outer card.

### Navigation
- **Style:** Fixed pill-shaped link targets (999px radius) with a translucent Signal-Teal hover/active fill; the brand mark uses the real logo asset, never a text wordmark substitute.
- **States:** Default → translucent teal background + Deep Navy text on hover/active.
- **Primary CTA:** Pill, Deep Navy fill, always present even when the link list collapses.
- **Mobile:** The link list (Problem / Shift / Model / Pillars / Proof) hides below 1100px; only the logo and the pill CTA remain down to the smallest viewport. There is no hamburger/drawer replacement — this is an accepted tradeoff, not an oversight, because the CTA always remains reachable.

### Signal / Status (signature component)
The operating-loop pulse — concentric SVG rings plus a Signal-Glow box-shadow — is the system's one signature device. It renders only on elements that represent something genuinely live (the hero's operating-loop diagram, a status dot), at a perfectly circular shape (50% radius), and never as a generic decorative accent elsewhere on the page.

## 6. Do's and Don'ts

### Do:
- **Do** keep Deep Navy (`#002D56`) as the dominant surface/text color; it is the system's base register, not an accent to be restrained.
- **Do** spend Precision Gold (`#ECAE3D`) on at most one or two moments per section — a stat figure, a status glow — per the Rare Gold Rule.
- **Do** render every register (display, body, technical label) in Archivo via weight/size/tracking/case changes, per the One Family Rule.
- **Do** keep structural panels at the 2–3px "drafting precision" radius, full pills (999px) for every interactive control, and true circles for status/signal elements — never mix the three.
- **Do** route the dominant, filled primary button to `#contact`; reserve the ghost/secondary button for exploratory in-page destinations.
- **Do** use only translucent tints of Ink or Instrument Mist for borders and dividers (Tinted Hairline Rule) — never a flat gray stroke.
- **Do** reserve the concentric Signal-Glow rings for things that are actually live or monitored (Signal-Glow Exception).
- **Do** ship every new animated element with a `prefers-reduced-motion: reduce` alternative, matching the coverage already present site-wide.

### Don't:
- **Don't** introduce gradients or glassmorphism as a default surface treatment. PRODUCT.md and CLAUDE.md both name this directly ("overuse of gradients," "excessive glassmorphism") — `backdrop-filter: blur()` currently exists on a small, closed set of components (the hero card, the scrolled nav); do not extend it to new components, and prefer the Ambient/Card shadow vocabulary instead.
- **Don't** add a tiny uppercase tracked eyebrow above every section as default scaffolding, or stamp 01/02/03 numbering onto cards that are parallel claims rather than a real sequence. The hero's three-step operating list is a genuine sequence and earns its numbers; a row of unrelated feature cards does not.
- **Don't** fabricate metrics, certifications, awards, or client names. Every figure and credential on the page must already exist in approved source copy — this is a content rule from PRODUCT.md, not a styling suggestion, and it applies equally to any new section a designer or agent adds.
- **Don't** add a second typeface for "editorial" contrast. The One Family Rule exists precisely so nobody reaches for a serif or a mono webfont to signal sophistication.
- **Don't** use a hard, tight, dark drop shadow anywhere. If a shadow needs more presence, reach for the Card shadow (larger blur, same low opacity), not a harder one.
- **Don't** let the spring/overshoot easing (`cubic-bezier(.34, 1.56, .64, 1)`) spread beyond the handful of small hover-icon nudges it already drives. It's in tension with an executive-ready, restraint-over-spectacle brand; exponential ease-out curves are the default for everything else.
- **Don't** add bloated dependencies or a build step. This is a single static `index.html`; every new pattern must work as plain CSS/JS dropped into that one file.
- **Don't** chase a design trend that will date the page in a year — this system is built to still look correct in five.
