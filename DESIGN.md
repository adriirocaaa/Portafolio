---
name: Cyber-Editorial Brutalism
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c5c9ac'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8f9378'
  outline-variant: '#444932'
  surface-tint: '#b0d500'
  primary: '#ffffff'
  on-primary: '#2a3400'
  primary-container: '#caf300'
  on-primary-container: '#596c00'
  inverse-primary: '#536600'
  secondary: '#c0c1ff'
  on-secondary: '#1000a9'
  secondary-container: '#3131c0'
  on-secondary-container: '#b0b2ff'
  tertiary: '#ffffff'
  on-tertiary: '#1b343d'
  tertiary-container: '#cde7f3'
  on-tertiary-container: '#506873'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#caf300'
  primary-fixed-dim: '#b0d500'
  on-primary-fixed: '#171e00'
  on-primary-fixed-variant: '#3e4c00'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#cde7f3'
  tertiary-fixed-dim: '#b1cad7'
  on-tertiary-fixed: '#041e28'
  on-tertiary-fixed-variant: '#324a54'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
  canvas-black: '#0a0a0a'
  paper-white: '#ffffff'
  cyber-lime: '#d4ff00'
  electric-indigo: '#6366f1'
  border-muted: '#262626'
  text-secondary: '#a1a1aa'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 120px
    fontWeight: '700'
    lineHeight: 110px
    letterSpacing: -0.04em
  display-xl-mobile:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: 60px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  body-lg:
    fontFamily: Space Grotesk
    fontSize: 20px
    fontWeight: '400'
    lineHeight: 32px
  body-md:
    fontFamily: Space Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  mono-label:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0.1em
  mono-code:
    fontFamily: Space Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
spacing:
  margin-page: 5vw
  gutter-grid: 2rem
  section-gap: 10rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
  stack-lg: 3rem
---

## Brand & Style

This design system embodies a "High-End Developer" persona through a fusion of **Brutalist-Minimalism** and editorial sophistication. It targets a tech-savvy audience that values precision, raw performance, and bespoke craftsmanship.

The aesthetic is characterized by:
- **High-Contrast Impact:** A stark dark-mode foundation that makes content pop with surgical precision.
- **Technical Honesty:** The use of monospaced fonts and grid-visible logic to celebrate the underlying code.
- **Aggressive Whitespace:** Generous margins and deliberate "voids" that elevate the content to an art-gallery status.
- **Raw Refinement:** Intentional use of grain, noise textures, and bold borders to create a tactile, physical-digital feel.

## Colors

The palette is anchored in a deep **Canvas Black** (#0a0a0a) to provide an infinite depth for editorial content. **Paper White** is used exclusively for primary text and high-contrast separators.

**Cyber Lime** is the lead functional accent, used for interactive elements, status indicators, and critical path CTAs. **Electric Indigo** serves as a secondary accent for code snippets, secondary metadata, or hover-state transitions. 

The color logic follows a high-contrast rule: if an element isn't vibrant lime or white, it should recede into the dark background using muted grays or subtle borders.

## Typography

Typography is the primary structural element of this design system. 
- **Space Grotesk** handles the heavy lifting, used in tight, high-impact weights for headlines and a legible, open weight for body copy.
- **Space Mono** acts as the technical "kicker" or metadata layer. It should be used for eyebrows, labels, and small UI details to reinforce the developer-centric aesthetic.

For editorial emphasis, use `italic` sparingly within headlines to create visual rhythm. Marquee elements should exclusively use **Space Mono** to mimic a terminal ticker.

## Layout & Spacing

The layout utilizes a **Fixed-Fluid Hybrid Grid**. Content is centered within a 12-column grid with a max-width of 1440px, but background elements and marquees bleed to the edge of the viewport.

**Breakpoints:**
- **Mobile (<768px):** 4-column grid, 16px margins, 16px gutters. Vertical spacing scales down by 50%.
- **Tablet (768px - 1024px):** 8-column grid, 40px margins.
- **Desktop (>1024px):** 12-column grid, dynamic viewport-based margins (5vw).

Vertical rhythm is intentionally loose; use "oversized" gaps between sections to create a premium, unhurried feel.

## Elevation & Depth

This system rejects soft shadows and blurs in favor of **Tonal Layers** and **Bold Outlines**. 

- **Surface Tiers:** The base is `canvas-black`. Cards and containers use a slightly elevated `surface-1` (near-black) or are defined by a 1px `border-muted`.
- **Noise Texture:** A global, low-opacity grain overlay is applied to the entire UI to prevent "flatness" and add a filmic quality.
- **Z-Index Strategy:** Depth is communicated through stacking order rather than light source. Fixed elements (like the custom cursor and navigation) sit on the highest plane, appearing to float over the content as it scrolls.

## Shapes

The shape language is strictly **Sharp (0px)**. All containers, buttons, and image wrappers use square corners to maintain the brutalist, architectural feel. 

Circular elements are reserved exclusively for "Status Dots" or custom cursor rings to provide a singular point of organic contrast against the rigid grid.

## Components

- **Buttons:** Use a solid `cyber-lime` background with `canvas-black` text for primary actions. Ghost buttons use a 1px white border with an arrow glyph (`→`). Hover states should invert colors or trigger a slight 2px offset.
- **Kickers (Eyebrows):** Small-caps **Space Mono** text paired with a leading dot or square, placed above main headlines.
- **Project Cards:** Large, full-bleed images or CSS-based mockups. On hover, the image should slightly scale or desaturate, revealing technical metadata in the corners.
- **Inputs:** Simple bottom-border only styling. Focus state transitions the border color to `cyber-lime` and moves the label upwards in **Space Mono**.
- **Marquees:** Constant-motion text ribbons using **Space Mono**. Use these to separate major sections or highlight the tech stack.
- **Custom Cursor:** A 10px `cyber-lime` dot with a trailing 40px hollow ring that expands when hovering over interactive elements.