---
name: IMS Sovereign
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#43474e'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#73777f'
  outline-variant: '#c3c6d0'
  surface-tint: '#3f608b'
  primary: '#001833'
  on-primary: '#ffffff'
  primary-container: '#002d56'
  on-primary-container: '#7596c4'
  inverse-primary: '#a7c8fa'
  secondary: '#7e5700'
  on-secondary: '#ffffff'
  secondary-container: '#febe4c'
  on-secondary-container: '#714d00'
  tertiary: '#001835'
  on-tertiary: '#ffffff'
  tertiary-container: '#002d58'
  on-tertiary-container: '#6396dc'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d4e3ff'
  primary-fixed-dim: '#a7c8fa'
  on-primary-fixed: '#001c39'
  on-primary-fixed-variant: '#254872'
  secondary-fixed: '#ffdead'
  secondary-fixed-dim: '#fbbb49'
  on-secondary-fixed: '#281900'
  on-secondary-fixed-variant: '#604100'
  tertiary-fixed: '#d4e3ff'
  tertiary-fixed-dim: '#a6c8ff'
  on-tertiary-fixed: '#001c3a'
  on-tertiary-fixed-variant: '#004786'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
  deep-navy: '#002D56'
  precision-gold: '#ECAE3D'
  technical-blue: '#004B8D'
  surface-white: '#FFFFFF'
  ink-charcoal: '#1A1A1A'
typography:
  display-lg:
    fontFamily: Source Serif 4
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Source Serif 4
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Source Serif 4
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Source Serif 4
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1280px
---

## Brand & Style

This design system is built for high-stakes enterprise environments where credibility and technical precision are paramount. The aesthetic moves away from "playful SaaS" toward a **Modern Corporate/Editorial** hybrid. It emphasizes authority through structured layouts, high-quality typography, and a "less-is-more" philosophy.

The visual language is characterized by:
- **Minimalism:** Use of generous, intentional whitespace to reduce cognitive load in complex data environments.
- **Precision:** Sharp, purposeful alignment and a strict adherence to the grid.
- **Human Connection:** Incorporating high-contrast editorial typography to signify thought leadership and heritage within a modern framework.
- **Reliability:** A solid, grounded color palette that avoids fleeting trends like neon gradients or heavy blurs.

## Colors

The palette is anchored in **Deep Navy** and **Ink Charcoal** to establish immediate institutional trust. 

- **Primary (Deep Navy):** Used for navigation, primary buttons, and structural headers to ground the interface.
- **Secondary (Precision Gold):** Reserved for high-value calls to action, success states, or subtle accents that guide the eye to key performance indicators.
- **Tertiary (Technical Blue):** Utilized for interactive elements like links and active states to provide clear affordance without breaking the professional tone.
- **Neutrals:** The background uses a "Crisp White" (`#FFFFFF`) with "Cool Gray" (`#F8F8F8`) for sectioning and containment to ensure the UI feels airy and organized.

## Typography

The system utilizes an editorial pairing to balance heritage with modernity.

- **Headlines (Source Serif 4):** This serif provides an authoritative, literary feel. It should be used for page titles, section headers, and impactful pull-quotes. Use tighter letter spacing for large display sizes to maintain a premium look.
- **Body & Interface (Hanken Grotesk):** A sharp, contemporary sans-serif designed for legibility in dense data applications. It handles high-density tables and technical labels with clarity.
- **Hierarchy:** Maintain a clear distinction between content (Serif) and utility (Sans-Serif). Labels and system feedback should always use the Sans-Serif at medium weights.

## Layout & Spacing

The layout follows a **Fixed-Fluid Hybrid** model. Content is contained within a max-width of 1280px to ensure readability on wide enterprise monitors, while using a 12-column grid for internal alignment.

- **Vertical Rhythm:** Built on an 8px baseline grid. Padding and margins should be increments of 8 (8, 16, 24, 32, 48, 64, 80).
- **Whitespace:** Use "Generous Padding" (48px+) between major sections to prevent the "dashboard clutter" common in B2B software.
- **Breakpoints:**
  - **Mobile (< 768px):** 4-column grid, 16px margins.
  - **Tablet (768px - 1024px):** 8-column grid, 24px margins.
  - **Desktop (> 1024px):** 12-column grid, 64px margins.

## Elevation & Depth

This design system avoids heavy drop shadows, opting instead for **Tonal Layering** and **Micro-Borders**.

- **Surface Tiers:** Use subtle background color shifts (e.g., White surface on a Cool Gray background) to denote elevation.
- **Low-Contrast Outlines:** Instead of shadows, use 1px borders in `#E5E5E5` for cards and containers.
- **Active Elevation:** When an element requires a shadow (like a dropdown or modal), use a very soft, high-diffusion "Ambient Shadow" with 4% opacity of the Deep Navy primary color. This creates a "lift" rather than a "float."
- **Focus States:** Use a 2px offset solid stroke in Technical Blue to highlight interactive elements for accessibility without cluttering the visual field.

## Shapes

The shape language is **Soft (0.25rem)** to maintain a professional, architectural feel. 

- **Primary Components:** Buttons, input fields, and small cards use a 4px (0.25rem) radius.
- **Large Containers:** Section containers and large cards may use "rounded-lg" (8px) to provide a slightly more approachable feel for high-level overview areas.
- **Strictness:** Avoid pill-shaped buttons or fully rounded icons. Keep edges defined to reinforce the brand's precision and technical depth.

## Components

- **Buttons:** Primary buttons use Deep Navy with white text. Secondary buttons use a Technical Blue outline. Avoid "ghost" buttons for primary actions; ensure high contrast at all times.
- **Input Fields:** Use a structured, "boxed" approach with 1px borders. Labels should be Hanken Grotesk 14px, positioned above the field for maximum legibility in forms.
- **Cards:** White backgrounds with 1px Light Gray borders. No shadows by default. Use Source Serif 4 for card titles to create an editorial feel.
- **Data Tables:** Highly functional. Use "Technical Blue" for header rows and "Cool Gray" for zebra-striping. Avoid vertical lines; use horizontal rules only to maintain an open, modern look.
- **Chips/Badges:** Use flat color fills with high-contrast text. For status indicators, use muted versions of Success (Green), Warning (Gold), and Error (Red) to keep them within the professional palette range.
- **Navigation:** A clean top-level bar using Deep Navy for high authority, or a left-rail sidebar for complex application navigation using the Cool Gray neutral.