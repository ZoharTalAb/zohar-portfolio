---
name: Precision Logic
colors:
  surface: '#0e1511'
  surface-dim: '#0e1511'
  surface-bright: '#343b36'
  surface-container-lowest: '#09100c'
  surface-container-low: '#161d19'
  surface-container: '#1a211d'
  surface-container-high: '#242c27'
  surface-container-highest: '#2f3632'
  on-surface: '#dde4dd'
  on-surface-variant: '#bbcabf'
  inverse-surface: '#dde4dd'
  inverse-on-surface: '#2b322d'
  outline: '#86948a'
  outline-variant: '#3c4a42'
  surface-tint: '#4edea3'
  primary: '#4edea3'
  on-primary: '#003824'
  primary-container: '#10b981'
  on-primary-container: '#00422b'
  inverse-primary: '#006c49'
  secondary: '#ffb95f'
  on-secondary: '#472a00'
  secondary-container: '#ee9800'
  on-secondary-container: '#5b3800'
  tertiary: '#ffb3af'
  on-tertiary: '#650911'
  tertiary-container: '#fc7c78'
  on-tertiary-container: '#711419'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#6ffbbe'
  primary-fixed-dim: '#4edea3'
  on-primary-fixed: '#002113'
  on-primary-fixed-variant: '#005236'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#ffdad7'
  tertiary-fixed-dim: '#ffb3af'
  on-tertiary-fixed: '#410005'
  on-tertiary-fixed-variant: '#842225'
  background: '#0e1511'
  on-background: '#dde4dd'
  surface-variant: '#2f3632'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-xl:
    fontFamily: Geist
    fontSize: 36px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Geist
    fontSize: 30px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '500'
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
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  headline-xl-mobile:
    fontFamily: Geist
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 16px
  section-gap: 80px
---

## Brand & Style

This design system is engineered for a senior backend developer persona, prioritizing technical sophistication over flashy trends. The brand personality is rooted in **expertise, stability, and clarity**. It avoids the cliché "hacker" aesthetics (neon cyans and matrix effects) in favor of a mature, high-contrast palette that suggests premium craftsmanship and architectural rigor.

The visual style utilizes a **Modern Glassmorphism** approach. This involves deep charcoal layers, subtle translucency, and precise borders that mimic the clean lines of a well-structured codebase. The emotional response should be one of immediate trust—positioning the developer as a reliable professional capable of handling complex enterprise systems.

## Colors

The palette is anchored by a deep **Graphite Base (#121212)** to reduce eye strain and provide a canvas for high-contrast elements. 

*   **Primary Emerald (#10b981):** Used for primary actions, success states, and key branding moments. It represents growth and systemic health.
*   **Warm Amber (#f59e0b):** Reserved for accentuation, warnings, and high-priority call-to-outs. This provides a warm counterpoint to the cool greens and dark grays.
*   **Neutrals:** Off-white text ensures maximum legibility without the harshness of pure white. Surfaces use a semi-transparent charcoal to create the glassmorphic depth.

## Typography

The typography system uses a tri-font approach to emphasize the "developer" identity while maintaining readability:

1.  **Geist (Headlines):** A technical, precise sans-serif that feels engineered. Used for all major headings.
2.  **Inter (Body):** The industry standard for UI legibility. Used for all long-form content and descriptions.
3.  **JetBrains Mono (Labels/Code):** A monospaced font used for tags, metadata, and actual code snippets to reinforce the backend focus.

Maintain generous line-height (1.6x) for body text to improve the reading experience for recruiters and technical managers.

## Layout & Spacing

This design system employs a **Fixed-Fluid Hybrid Grid**. Content is centered within a 1200px maximum container on desktop to ensure line lengths remain readable. 

*   **Grid:** A 12-column grid is used for desktop, collapsing to 4 columns on mobile.
*   **Spacing Rhythm:** An 8px linear scale (8, 16, 24, 32, 48, 64, 80) governs all margins and paddings.
*   **White Space:** Significant vertical spacing (80px+) between sections is mandatory to evoke a "premium" and "uncluttered" feel, mimicking high-end architectural sites.

## Elevation & Depth

Depth is achieved through **Glassmorphism and Tonal Layering** rather than traditional heavy shadows.

*   **Background:** The base layer is #121212.
*   **Surface (Card/Nav):** Use `rgba(30, 30, 30, 0.6)` with a `backdrop-filter: blur(12px)`. This creates the frosted glass effect.
*   **Borders:** Every glass element must have a 1px solid border using `rgba(255, 255, 255, 0.1)`. This "inner glow" border is critical for defining edges in dark mode.
*   **Shadows:** Use a single, extremely soft ambient shadow for floating elements: `0 20px 40px rgba(0, 0, 0, 0.4)`.

## Shapes

The shape language is **Structured and Refined**. We use a "Rounded" (Level 2) setting:
*   Standard components (Buttons, Inputs) use a **0.5rem (8px)** corner radius.
*   Containers and Cards use **1rem (16px)** to provide a softer, more modern container for the technical content.
*   The 8px radius maintains a balance between "industrial/precise" and "friendly/modern."

## Components

### Buttons
*   **Primary:** Solid Emerald (#10b981) background with near-black text. High contrast is essential for the CTA.
*   **Secondary/Ghost:** 1px border of `rgba(255, 255, 255, 0.2)` with white text. On hover, background becomes `rgba(255, 255, 255, 0.05)`.

### Cards
*   Cards must use the glassmorphic style: semi-transparent surface, backdrop blur, and the 1px subtle border. 
*   Interactive cards should have a subtle Emerald border-color shift on hover.

### Input Fields
*   Dark backgrounds (#1a1a1a) with 1px borders. 
*   The focus state should use a 1px Emerald border and a very subtle Emerald outer glow (2px spread).

### Chips & Tags
*   Use JetBrains Mono for the text. 
*   Small 4px radius. 
*   Backgrounds should be low-contrast (e.g., `rgba(16, 185, 129, 0.1)`) with primary-colored text.

### Progress/Stats
*   Use Emerald for "Active" or "Healthy" metrics.
*   Use Amber for "In Progress" or "Optimization Needed" metrics.
*   Data visualizations should be clean, using thin strokes and no fills where possible.