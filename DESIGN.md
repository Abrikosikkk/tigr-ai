---
name: Lustrous Intelligence
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c5c6cb'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8e9195'
  outline-variant: '#44474a'
  surface-tint: '#c1c7cf'
  primary: '#ffffff'
  on-primary: '#2b3137'
  primary-container: '#dde3eb'
  on-primary-container: '#5f656c'
  inverse-primary: '#595f66'
  secondary: '#b9c8de'
  on-secondary: '#233143'
  secondary-container: '#39485a'
  on-secondary-container: '#a7b6cc'
  tertiary: '#ffffff'
  on-tertiary: '#3a3000'
  tertiary-container: '#ffe16d'
  on-tertiary-container: '#776300'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dde3eb'
  primary-fixed-dim: '#c1c7cf'
  on-primary-fixed: '#161c22'
  on-primary-fixed-variant: '#41474e'
  secondary-fixed: '#d4e4fa'
  secondary-fixed-dim: '#b9c8de'
  on-secondary-fixed: '#0d1c2d'
  on-secondary-fixed-variant: '#39485a'
  tertiary-fixed: '#ffe16d'
  tertiary-fixed-dim: '#e9c400'
  on-tertiary-fixed: '#221b00'
  on-tertiary-fixed-variant: '#544600'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  headline-xl:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Manrope
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1440px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style
The brand personality is high-end, intellectual, and technologically advanced. It targets a sophisticated audience that values precision and premium aesthetics. The UI evokes a sense of "Lustrous Intelligence"—where data feels like light passing through crystal.

The design style is a refined **Glassmorphism** mixed with **Minimalism**. It utilizes frosted surfaces, delicate light refraction, and metallic accents to create a sense of depth and quality. Surfaces should feel like machined aluminum or polished glass, providing a professional yet futuristic atmosphere for complex administrative and authentication workflows.

## Colors
This design system utilizes a "Silver & Slate" palette to achieve a metallic, premium feel. 
- **Primary (#E2E8F0):** A bright, cool silver used for high-emphasis text and interactive states.
- **Secondary (#94A3B8):** A muted steel blue-grey for secondary information and iconography.
- **Tertiary (#FFD700):** A selective "Gold" accent used exclusively for high-tier features like the "Pupkin+" badge and specialized administrative alerts.
- **Neutral (#0F172A):** A deep, midnight slate that serves as the void behind the glass surfaces.

For **Glassmorphism**, use semi-transparent whites (e.g., `rgba(255, 255, 255, 0.05)`) for background fills and high-clarity blurs.

## Typography
The typography strategy blends the modern elegance of **Manrope** for headings with the technical precision of **Geist** for body text. 

For administrative functions, such as "Key Generation" or "User Management" tables, **JetBrains Mono** is employed for labels and data strings to emphasize the "Intelligence" aspect of the brand. Headings should utilize tighter letter spacing to maintain a "machined" look, while mono labels should be spaced out for maximum legibility in complex UI layouts.

## Layout & Spacing
The layout follows a **Fluid Grid** model with a maximum container width to maintain readability on ultra-wide monitors. 

- **Desktop:** 12-column grid with 24px gutters. Use large internal padding (48px+) for glass containers to let the background blur breathe.
- **Mobile:** 4-column grid with 16px margins.
- **Rhythm:** Use a 4px base unit. Administrative tables and user management views should use a compact density (`stack-sm`) to display high volumes of data, while authentication screens should use a "Spacious" density (`stack-lg`) to focus user attention.

## Elevation & Depth
Depth is achieved through **Glassmorphism** and light refraction rather than traditional shadows.
- **Level 1 (Base):** Deep Slate background.
- **Level 2 (Panels):** `rgba(255, 255, 255, 0.03)` fill with a `20px` backdrop-blur. 1px solid border at `rgba(255, 255, 255, 0.1)`.
- **Level 3 (Modals/Popovers):** `rgba(255, 255, 255, 0.08)` fill with `40px` backdrop-blur. A "Light Leak" effect is applied to the top-left corner using a subtle white gradient to simulate a metallic edge.
- **Shadows:** Use extremely diffused, low-opacity shadows (`rgba(0,0,0,0.4)`) only to separate Level 3 elements from Level 2.

## Shapes
The shape language is "Sophisticated Geometric." 
- **Standard (0.5rem):** Used for input fields, buttons, and administrative cards.
- **Large (1rem):** Used for main dashboard containers and authentication modals.
- **Pill:** Used exclusively for status indicators (Active/Inactive) and the "Pupkin+" subscription badge.
- **Borders:** All glass elements must have a 1px inner stroke to define their silhouette against the dark background.

## Components
### Authentication (Login/Signup)
Centered glass containers with high backdrop blur. Primary buttons use a metallic silver gradient. Input fields are dark with semi-transparent borders that glow slightly on focus.

### Subscription Badges (Pupkin+)
A pill-shaped component with a metallic silver-to-white gradient background. Text should be black or dark slate for maximum contrast. A subtle "shimmer" animation should trigger on hover to emphasize the premium nature.

### Administrative UI
- **Key Generation:** Use a monospaced "Key Display" component with a "Click to Copy" interaction. The generated key should appear in a recessed, high-contrast block.
- **User Management:** High-density tables with subtle row separators (`rgba(255,255,255,0.05)`). Actions (Edit/Delete) should be secondary-colored icons that turn primary-colored on hover.
- **Buttons:** Primary buttons use the Silver gradient. Secondary buttons use a "Ghost" style with a 1px metallic border.
- **Inputs:** Understated dark fills. Error states use a thin red outer glow rather than a solid background change to preserve the glass effect.