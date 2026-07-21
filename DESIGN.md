---
name: Obsidian Apex
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
  on-surface-variant: '#ddc1ae'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#a48c7a'
  outline-variant: '#564334'
  surface-tint: '#ffb77d'
  primary: '#ffb77d'
  on-primary: '#4d2600'
  primary-container: '#ff8c00'
  on-primary-container: '#623200'
  inverse-primary: '#904d00'
  secondary: '#ffe2ab'
  on-secondary: '#402d00'
  secondary-container: '#ffbf00'
  on-secondary-container: '#6d5000'
  tertiary: '#b7c8e1'
  on-tertiary: '#213145'
  tertiary-container: '#9babc4'
  on-tertiary-container: '#304054'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdcc3'
  primary-fixed-dim: '#ffb77d'
  on-primary-fixed: '#2f1500'
  on-primary-fixed-variant: '#6e3900'
  secondary-fixed: '#ffdfa0'
  secondary-fixed-dim: '#fbbc00'
  on-secondary-fixed: '#261a00'
  on-secondary-fixed-variant: '#5c4300'
  tertiary-fixed: '#d3e4fe'
  tertiary-fixed-dim: '#b7c8e1'
  on-tertiary-fixed: '#0b1c30'
  on-tertiary-fixed-variant: '#38485d'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-xl:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
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
  container-padding: 20px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 24px
  gutter: 16px
---

## Brand & Style
The design system is centered on the intersection of primal energy and advanced intelligence. It caters to a high-intent audience that values efficiency, speed, and a premium aesthetic. The visual narrative combines **Modern Minimalism** with **Glassmorphism** to create a high-tech environment that feels both sophisticated and hyper-functional.

The emotional response should be one of focused power—the "stealth" of a predator combined with the clarity of a modern workspace. Surfaces are deep and immersive, allowing the vibrant amber accents to guide the user's eye toward primary actions and AI-driven insights. The aesthetic is clean, omitting unnecessary ornamentation in favor of structural clarity and refined transparency.

## Colors
The palette is rooted in a deep obsidian foundation to ensure maximum contrast for the AI interface.

- **Primary (Tiger Orange):** `#FF8C00` – Used for primary call-to-actions, active states, and brand-critical indicators.
- **Secondary (Amber):** `#FFBF00` – Used for highlights, subtle gradients, and differentiating AI-generated content.
- **Tertiary (Slate Gray):** `#64748B` – Utilized for metadata, inactive icons, and secondary text to maintain a calm hierarchy.
- **Neutral (Obsidian):** `#0A0A0A` – The core background color, providing a pure, deep-space canvas.
- **Surface (Glass):** `rgba(255, 255, 255, 0.05)` – Used for glassmorphic containers with a backdrop blur of 12px-20px.

## Typography
The typography system uses a dual-font approach to balance brand character with technical legibility. 

**Montserrat** is reserved for headlines and display elements, providing a geometric, confident personality. **Inter** is the workhorse for all body text, chat bubbles, and labels, selected for its exceptional readability on mobile displays and its neutral, systematic feel. 

Large display type should use tighter letter spacing to feel more "custom" and premium. All labels should be set in uppercase when used for navigation or small UI metadata to enhance the sophisticated, technical vibe.

## Layout & Spacing
This design system utilizes a **Fluid Grid** model optimized for mobile-first interaction. The core spacing logic is built on a 4px baseline grid to ensure mathematical harmony between elements.

- **Margins:** 20px horizontal margins for the main content area to provide breathing room on narrow devices.
- **Chat Layout:** Messages follow a staggered vertical stack with 12px spacing between bubbles from the same sender and 24px between different senders.
- **Safe Areas:** Strict adherence to bottom-sheet and notch safe areas is required, with interactive elements (like the chat input) pinned to the bottom of the screen with a glassmorphic background.

## Elevation & Depth
Depth is created through **Tonal Layering** and **Glassmorphism** rather than traditional heavy shadows.

- **Level 0 (Background):** Pure Obsidian `#0A0A0A`.
- **Level 1 (Cards/Bubbles):** `rgba(255, 255, 255, 0.03)` with a 1px stroke of `rgba(255, 255, 255, 0.1)`.
- **Level 2 (Active Overlays/Modals):** Glassmorphic surfaces with `backdrop-filter: blur(20px)` and a soft amber ambient glow (`rgba(255, 140, 0, 0.15)`) instead of a black shadow.
- **Refined Shadow Play:** Use very large, low-opacity shadows (20% opacity, 40px blur) to lift primary buttons slightly off the surface, making them feel like they are floating in a dark room.

## Shapes
The shape language is modern and approachable, utilizing a **Rounded** (0.5rem base) philosophy but pushing toward larger radii for primary containers.

- **Chat Bubbles:** 1.5rem (`rounded-xl`) to feel friendly and fluid.
- **Buttons:** Fully pill-shaped for high-priority actions.
- **Input Fields:** 1rem (`rounded-lg`) for a stable, grounded look.
- **Icons:** Use a 1.5pt or 2pt stroke width with rounded caps and joins to match the UI's softness.

## Components
- **Buttons:** Primary buttons are solid Tiger Orange with white or black text. Secondary buttons use a "Ghost" style with a 1px amber border and glass background.
- **Chat Bubbles:** User messages are Obsidian with a Slate border. AI messages use a subtle Glassmorphic background with a soft Amber left-accent border to signify intelligence.
- **Input Field:** A wide, pill-shaped glass container. The "Send" button should be a circular icon button that remains disabled (low opacity) until text is entered.
- **Chips:** Small, pill-shaped elements used for "Suggested Prompts." These should have a slight `0.05` white fill and a 0.5px border to stand out against the background.
- **AI Pulse:** A custom component—a glowing amber ring or orb—should be used to indicate when the AI is "thinking," using a breathing animation (scale and opacity).
- **Cards:** Used for rich media or tool results, featuring a `rounded-xl` corner radius and a subtle internal glow.