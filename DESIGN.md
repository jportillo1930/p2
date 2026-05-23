---
name: Cyber-Minimalist Portfolio
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#b9ccb2'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#84967e'
  outline-variant: '#3b4b37'
  surface-tint: '#00e639'
  primary: '#ebffe2'
  on-primary: '#003907'
  primary-container: '#00ff41'
  on-primary-container: '#007117'
  inverse-primary: '#006e16'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#fff8f4'
  on-tertiary: '#442b10'
  tertiary-container: '#ffd5ae'
  on-tertiary-container: '#7a5b3c'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#72ff70'
  primary-fixed-dim: '#00e639'
  on-primary-fixed: '#002203'
  on-primary-fixed-variant: '#00530e'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#ffdcbd'
  tertiary-fixed-dim: '#e7bf99'
  on-tertiary-fixed: '#2c1701'
  on-tertiary-fixed-variant: '#5d4124'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display:
    fontFamily: Geist
    fontSize: 84px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  base: 8px
  xs: 4px
  sm: 16px
  md: 32px
  lg: 64px
  xl: 128px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 80px
---

## Brand & Style

This design system is built for a high-performance developer persona, blending extreme minimalism with a "Matrix-inspired" high-tech aesthetic. The brand personality is precise, technical, and authoritative. It strips away unnecessary ornamentation to focus on raw information and code-driven interactions.

The visual style is a hybrid of **Minimalism** and **Modern Brutalism**, utilizing a strict monochromatic foundation. Depth is achieved not through shadows, but through structural lines and vibrant, glowing green accents that simulate a terminal interface. The goal is to evoke a sense of digital craftsmanship and "low-level" engineering mastery.

## Colors

The palette is intentionally restricted to maintain a sleek, professional "hacker" aesthetic. 

- **Backgrounds:** Absolute black (#000000) serves as the void, providing maximum contrast for text and glowing elements.
- **Primary:** "Matrix Green" (#00FF41) is used exclusively for interactive states, code highlights, and "floating" terminal effects. It should be treated as a luminous light source.
- **Typography:** Pure white (#FFFFFF) for primary headers to ensure legibility, with muted grays for secondary information to maintain hierarchy.
- **Accents:** Use subtle dark greys for structural elements like borders and container backgrounds to prevent the UI from feeling flat.

## Typography

The typography strategy focuses on the contrast between high-impact sans-serif headings and functional monospaced data.

- **Headlines:** Use **Geist** in bold or extra-bold weights. The tight letter spacing and geometric construction reinforce the minimalist, modern feel.
- **Body:** **Inter** provides high legibility for project descriptions and bio sections, offering a neutral balance to the more aggressive headlines.
- **Code & Labels:** **JetBrains Mono** is utilized for all "technical" data, including tags, code snippets, and small metadata. This reinforces the developer-centric nature of the design system.

## Layout & Spacing

This design system employs a **fixed grid** approach for desktop to create a structured, "modular" feel. 

- **Grid:** A 12-column grid with a maximum content width of 1200px. Elements should feel like they are "slotted" into a technical blueprint.
- **Spacing Rhythm:** Use an 8px base unit. Large sections are separated by significant vertical whitespace (64px or 128px) to emphasize the minimalist aesthetic.
- **Borders as Spacers:** Instead of using background fills to separate content, use 1px solid lines (#222222) to create a "schematic" look.
- **Mobile:** Transition to a single-column layout with 20px side margins, maintaining the 8px vertical rhythm.

## Elevation & Depth

In this design system, depth is not simulated with realistic shadows. Instead, it uses **Tonal Layers** and **Luminous Accents**:

- **Surfaces:** The base layer is #000000. Secondary containers (like cards or code blocks) use a slightly lighter #0A0A0A surface with a 1px border.
- **Outlines:** Use "low-contrast outlines" (#222222) for inactive states. For active or hovered states, the outline should switch to the primary green (#00FF41).
- **Glow Effects:** Interactive elements (buttons, active tabs) use a soft outer glow (`box-shadow: 0 0 15px rgba(0, 255, 65, 0.3)`) to simulate a CRT or LED display.
- **Backdrop:** Background "matrix" code effects should be rendered at 5-10% opacity, appearing as if they are sitting "behind" the UI glass.

## Shapes

To maintain a high-tech, architectural feel, this design system uses **Sharp (0px)** corners for all primary UI elements. 

Rectilinear shapes reinforce the "terminal" and "monolithic" concept. Do not use border-radii on buttons, cards, or input fields. The only exception is for circular elements such as status indicators or specific iconography that requires organic forms.

## Components

- **Buttons:** Primary buttons are sharp-edged boxes with a 1px white border and white text. On hover, the background fills with #00FF41 and text switches to #000000.
- **Code Blocks:** Use a #0A0A0A background with a top bar displaying "terminal" controls (three small dots). Text is strictly JetBrains Mono in #00FF41.
- **Cards:** Simple 1px #222222 borders with no background fill. On hover, the border becomes white or green to indicate focus.
- **Chips/Tags:** Monospaced text inside a small 1px box. These should look like hardware labels.
- **Input Fields:** Bottom-border only (#222222) which transforms into a full-box green border when focused. Use a blinking "block" cursor (`|` or `_`) for the placeholder.
- **Status Indicators:** A small #00FF41 circle with a "pulse" animation to indicate "Available for Work" or "System Live."
- **Navigation:** Vertical navigation on the left side or a fixed header with "breadcrumb" style indicators (e.g., `PORTILLO > PROJECTS > 01`).