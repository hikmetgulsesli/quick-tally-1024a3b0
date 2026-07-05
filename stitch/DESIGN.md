---
name: Quick Tally
colors:
  surface: '#f9f9ff'
  surface-dim: '#d3daef'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e9edff'
  surface-container-high: '#e1e8fd'
  surface-container-highest: '#dce2f7'
  on-surface: '#141b2b'
  on-surface-variant: '#424656'
  inverse-surface: '#293040'
  inverse-on-surface: '#edf0ff'
  outline: '#727687'
  outline-variant: '#c2c6d8'
  surface-tint: '#0054d6'
  primary: '#0050cb'
  on-primary: '#ffffff'
  primary-container: '#0066ff'
  on-primary-container: '#f8f7ff'
  inverse-primary: '#b3c5ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#a33200'
  on-tertiary: '#ffffff'
  tertiary-container: '#cc4204'
  on-tertiary-container: '#fff6f4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae1ff'
  primary-fixed-dim: '#b3c5ff'
  on-primary-fixed: '#001849'
  on-primary-fixed-variant: '#003fa4'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdbd0'
  tertiary-fixed-dim: '#ffb59d'
  on-tertiary-fixed: '#390c00'
  on-tertiary-fixed-variant: '#832600'
  background: '#f9f9ff'
  on-background: '#141b2b'
  surface-variant: '#dce2f7'
typography:
  display-tally:
    fontFamily: Geist
    fontSize: 80px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Geist
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
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: Geist
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
  container-max: 1200px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style
The brand personality is rooted in precision, efficiency, and reliability. This design system treats the interface as a high-performance utility—a professional tool where every pixel serves a functional purpose. The aesthetic is **Minimalist-Technical**, prioritizing clarity over decoration to ensure users can perform counting and data tracking tasks with zero cognitive load.

The target audience consists of professionals in inventory management, research, and logistics who require a deterministic interface that responds instantly. The emotional response should be one of "controlled focus"—the UI stays out of the way until needed, providing a calm, uncluttered environment for high-accuracy work.

## Colors
The palette is dominated by a range of functional greyscale tones to establish a hierarchy of information without visual noise.

- **Primary (Tech Blue):** Used exclusively for the most important actions, primary buttons, and active focus states.
- **Secondary (Emerald Green):** Reserved for "success" indicators, increment confirmations, and completed tallies.
- **Neutral (Slate/Ink):** A range of cool-toned greys used for text, borders, and icon states to maintain a professional, technical feel.
- **Surface Strategy:** The design system uses a "Layered White" approach. The base background is slightly off-white (`#F9FAFB`) to reduce glare, while functional cards and inputs are pure white (`#FFFFFF`) to pop forward.

## Typography
The typography system uses **Geist** for structural elements and **Inter** for long-form reading. Geist’s geometric precision reinforces the "professional tool" aesthetic, while Inter provides familiar readability for labels and body text.

A specialized `display-tally` role is defined for the central counter numbers; it uses tight letter spacing and a semi-bold weight to command immediate attention. Tabular figures (`tnum`) must be enabled for all numerical data to prevent horizontal "jumping" as counts increment.

## Layout & Spacing
The layout follows a **Fixed-Fluid Hybrid** model. On desktop, the main content area is capped at 1200px and centered. On mobile, the layout is fluid with 16px side margins.

A strict 4px base grid governs all spatial decisions. Vertical rhythm is maintained through three primary "stack" tokens:
- **Stack-SM (8px):** For grouping related items like a label and its input.
- **Stack-MD (16px):** The default gap between independent UI components.
- **Stack-LG (32px):** Used to separate major sections or distinct data groups.

Components should utilize an "internal-first" padding strategy, ensuring that touch targets for tally buttons are large (minimum 48px height) even when the visual element appears compact.

## Elevation & Depth
This design system avoids heavy shadows, opting instead for **Tonal Layers** and **Low-Contrast Outlines**.

Depth is communicated through:
1.  **Z0 (Background):** The base canvas (`#F9FAFB`).
2.  **Z1 (Surface):** White cards with a 1px solid border in a soft neutral (`#E5E7EB`). No shadow.
3.  **Z2 (Interaction):** When an element is hovered or active, it gains a subtle, highly diffused ambient shadow (4px blur, 4% opacity) and the border color darkens slightly.
4.  **Z3 (Overlays):** Modals or dropdowns use a 1px border and a crisp, medium-depth shadow to signify temporary placement over the main interface.

## Shapes
In line with the utility focus, shapes use a **Soft (0.25rem)** roundedness. This provides just enough approachable "friendliness" to prevent the UI from feeling hostile or overly technical, while maintaining the sharp, efficient look of a modern SaaS tool.

- **Standard Buttons/Inputs:** 0.25rem (4px).
- **Cards/Containers:** 0.5rem (8px).
- **Feedback Toasts:** 0.75rem (12px) to distinguish them as floating notifications.
- **Icons:** Use a 1.5pt or 2pt stroke width with slightly rounded caps to match the font geometry.

## Components
- **Primary Buttons:** High-contrast Blue background with White text. No gradients. On-press, the color shifts 10% darker.
- **Tally Controls:** Large, centered cards featuring the `display-tally` type. Increment (+) and Decrement (-) buttons should be positioned at the bottom for easy thumb access on mobile, utilizing the full width of the card.
- **Toggle Switches:** Small, pill-shaped tracks with a white circular handle. Use Tech Blue for the 'On' state. Transitions must be instant (150ms) to feel responsive.
- **Input Fields:** Minimalist design with a 1px neutral border. Upon focus, the border transitions to Tech Blue with a subtle 2px outer glow (halo) in the same color at 20% opacity.
- **Chips/Status Tags:** Use a light grey background with `label-caps` typography. Success states use a Secondary Green tint for both text and background.
- **Data Lists:** High-density rows with 1px bottom dividers. Use `mono-data` for all numerical values to ensure vertical alignment across rows.