---
name: Quick Tally Utility System
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#464555'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#7e3000'
  on-tertiary: '#ffffff'
  tertiary-container: '#a44100'
  on-tertiary-container: '#ffd2be'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb695'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7b2f00'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-tally:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 36px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  container-max: 1280px
  gutter: 16px
---

## Brand & Style

The design system is a high-performance utility framework built for precision, speed, and clarity. It targets users who require immediate data entry and status monitoring without cognitive overhead. The aesthetic is **Minimalist / Tool-First**, prioritizing function over decoration.

The emotional response should be one of competence and reliability. By utilizing a "Slate and Zinc" monochromatic foundation, the interface recedes to let the user's data take center stage. Every element is intentional, stripping away marketing-led embellishments in favor of a workspace that feels like a professional instrument. 

Key principles:
- **Functional Clarity:** Information hierarchy is dictated by data importance.
- **Precision:** Tight alignment and consistent spacing to imply order.
- **Action-Oriented:** Use of color is strictly reserved for interaction and status changes.

## Colors

The palette is anchored in a professional scale of grays to provide a neutral environment for data density. 

- **Primary (Indigo):** Reserved exclusively for primary calls-to-action, active states, and critical focus indicators. It provides a high-contrast "signal" against the muted background.
- **Neutral (Slate/Zinc):** A range of cool grays used for backgrounds (`#F8FAFC`), borders (`#E2E8F0`), and secondary text (`#64748B`).
- **Surface:** The primary app surface is white (`#FFFFFF`) to ensure maximum legibility for small-scale typography and status numbers.
- **Semantic:** Success and Error colors are used sparingly for immediate feedback on tally operations.

## Typography

The design system utilizes **Inter** exclusively to leverage its exceptional legibility and systematic appearance. 

- **Data Numbers:** For tallies and counts, use `display-tally` with tabular figures enabled (`tnum`) to ensure numbers align vertically when scanning lists.
- **Hierarchy:** Use `label-caps` for metadata and non-interactive descriptors to differentiate them from actionable body text.
- **Contrast:** Maintain high contrast ratios (minimum 4.5:1) for all body text against the neutral backgrounds.

## Layout & Spacing

This design system uses a **4px baseline grid** to ensure mathematical precision in element alignment.

- **Grid Model:** A 12-column fluid grid for desktop, transitioning to a single-column stack for mobile. Gutters are fixed at 16px to maintain a compact, tool-like feel.
- **Density:** The layout favors "Compact" density. Vertical rhythm is tight, with 8px or 16px separating related form elements.
- **Safe Areas:** Generous outer margins (24px on desktop, 16px on mobile) prevent the interface from feeling cluttered at the edges of the viewport.

## Elevation & Depth

To maintain a minimalist aesthetic, depth is communicated through **Low-contrast outlines** rather than heavy shadows.

- **Surface Tiers:** Backgrounds use `#F8FAFC`, while cards and input areas use `#FFFFFF`.
- **Borders:** 1px solid borders in `#E2E8F0` define the structure.
- **Active Elevation:** Only the primary active element (e.g., a focused input or an active tally card) may receive a subtle, tinted shadow: `0 4px 12px rgba(79, 70, 229, 0.08)`.
- **Transitions:** Use immediate or very fast (150ms) transitions for hover states to reinforce the "snappy" utility nature of the tool.

## Shapes

The shape language is "Soft" yet disciplined. 

- **Base Radius:** 4px (0.25rem) for standard components like buttons and inputs.
- **Container Radius:** 8px (0.5rem) for cards and modals.
- **Consistency:** Avoid pill-shaped buttons; the rectangular forms with slight rounding reinforce the professional, grid-based layout of the design system.

## Components

### Buttons
- **Primary:** Solid Indigo (`#4F46E5`) with White text. No gradients.
- **Secondary:** White background with a 1px Slate border.
- **Icon Buttons:** Square 32x32px or 40x40px containers with centered icons, used for rapid tally increments.

### Status Cards
- Compact modules with a 1px border.
- Large numerical displays using `display-tally`.
- Contextual icons in the top-right corner to indicate status (trending up/down).

### Inputs & Toggles
- **Inputs:** 1px border that shifts to Indigo on focus. No inner shadows.
- **Toggles:** Small, rectangular switches. Gray for off, Indigo for on.
- **Checkboxes:** Square with a 2px radius; high-contrast checkmark.

### Progress Indicators
- Linear bars only. 4px height. Slate background with Indigo fill.

### List Items
- Tight vertical padding (12px). Separated by 1px Slate hairlines. Highly scannable with data right-aligned.