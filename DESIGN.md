---
name: Heritage Earth
colors:
  surface: '#fff8f5'
  surface-dim: '#e1d8d4'
  surface-bright: '#fff8f5'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fbf2ed'
  surface-container: '#f5ece7'
  surface-container-high: '#efe6e2'
  surface-container-highest: '#e9e1dc'
  on-surface: '#1e1b18'
  on-surface-variant: '#56433c'
  inverse-surface: '#34302c'
  inverse-on-surface: '#f8efea'
  outline: '#89726a'
  outline-variant: '#dcc1b7'
  surface-tint: '#9b441e'
  primary: '#893711'
  on-primary: '#ffffff'
  primary-container: '#a84e27'
  on-primary-container: '#ffe3d9'
  inverse-primary: '#ffb599'
  secondary: '#825500'
  on-secondary: '#ffffff'
  secondary-container: '#fdb64b'
  on-secondary-container: '#704800'
  tertiary: '#51504d'
  on-tertiary: '#ffffff'
  tertiary-container: '#6a6864'
  on-tertiary-container: '#ece8e3'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbce'
  primary-fixed-dim: '#ffb599'
  on-primary-fixed: '#370e00'
  on-primary-fixed-variant: '#7c2e07'
  secondary-fixed: '#ffddb3'
  secondary-fixed-dim: '#ffb951'
  on-secondary-fixed: '#291800'
  on-secondary-fixed-variant: '#633f00'
  tertiary-fixed: '#e6e2dd'
  tertiary-fixed-dim: '#c9c6c1'
  on-tertiary-fixed: '#1c1c19'
  on-tertiary-fixed-variant: '#484743'
  background: '#fff8f5'
  on-background: '#1e1b18'
  surface-variant: '#e9e1dc'
  terracotta: '#A84E27'
  amber: '#FFB84D'
  cream: '#F9F5F0'
  charcoal: '#2D2926'
  clay-muted: '#D9C5B2'
  success-green: '#4A6741'
typography:
  headline-xl:
    fontFamily: Source Serif 4
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Source Serif 4
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Source Serif 4
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
  headline-md:
    fontFamily: Source Serif 4
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  section-gap: 80px
---

## Brand & Style

This design system blends **Minimalism** with **Modern Corporate** sensibilities, tailored for a cultural heritage context. It aims to evoke a sense of "digital preservation"—balancing the warmth of historical artifacts with the precision of modern augmented reality technology.

The aesthetic is defined by its use of rich, organic tones and generous whitespace to create a premium, editorial feel. By combining high-contrast serif headlines with a functional sans-serif body, the interface communicates both the authority of a museum and the reliability expected by professional recruiters. Visual interest is maintained through subtle, culturally-inspired geometric patterns and soft, tonal layering rather than aggressive shadows or gradients.

## Colors

The palette is derived from the natural materials and pigments found in Malawi heritage artifacts. 

- **Primary (Terracotta):** Used for key actions and primary brand moments. It carries the weight of history and clay.
- **Secondary (Amber):** An accent for highlights, secondary CTAs, and signaling interactivity or "scanning" states.
- **Tertiary (Cream):** The primary surface color. It replaces pure white to reduce eye strain and provide a parchment-like warmth.
- **Neutral (Charcoal):** Used for typography and deep structural elements to ensure high contrast and legibility.

Avoid pure black or pure white; every surface should feel "dyed" or "organic."

## Typography

This system uses a **High-Contrast Pair**:
1. **Source Serif 4** for headings to provide an authoritative, literary, and historical feel. It suggests a curated museum experience.
2. **Plus Jakarta Sans** for body and labels. Its soft, modern curves ensure the app feels contemporary and accessible on digital screens.

**Hierarchy Rules:**
- Use `headline-xl` only for Hero sections.
- `label-md` should be used for section headers or small caps subtitles to add an "archival" feel.
- Maintain generous line heights (1.5x for body) to improve readability for academic and professional audiences.

## Layout & Spacing

The design system utilizes a **12-column fixed grid** for desktop and a **fluid single-column** layout for mobile. 

- **Desktop:** 1200px max-width, centered. 24px gutters.
- **Mobile:** 16px side margins.
- **Rhythm:** All spacing (padding, margins) must be multiples of the **8px base unit**.
- **Sectioning:** Large vertical gaps (80px+) are encouraged to separate the narrative flow of the landing page, allowing the artifacts and information to "breathe."

## Elevation & Depth

To maintain the "Modern Museum" feel, we avoid traditional shadows. Depth is communicated through:

- **Tonal Layering:** Using slightly darker or lighter variations of the `Cream` and `Clay` palette to stack surfaces.
- **Soft Outlines:** 1px borders in `clay-muted` (low opacity) define containers without adding visual weight.
- **Glassmorphism (Subtle):** For overlays or navigation bars, use a backdrop blur with a semi-transparent `Cream` fill to maintain context of the background "exhibit."
- **Focus States:** Use the `Amber` secondary color as a subtle outer glow or high-contrast border for interactive elements.

## Shapes

The shape language is **Rounded**, reflecting the organic nature of handcrafted pottery and wooden artifacts. 

- **Cards & Inputs:** 0.5rem (8px) radius.
- **Large Sections/Hero Images:** 1rem (16px) radius to create a soft, welcoming frame.
- **Pill Shapes:** Used exclusively for tags, chips, and small status indicators to differentiate them from functional buttons.
- **Cultural Patterns:** Use subtle SVG pattern fills (dots, weaves, or geometric chevrons) in 5% opacity charcoal on cream backgrounds to add texture.

## Components

### Buttons
- **Primary:** Terracotta background, Cream text, Semi-bold Plus Jakarta Sans. No shadow, flat color.
- **Secondary:** Transparent background, Terracotta border (2px), Terracotta text.
- **Download CTA:** Amber background, Charcoal text. Use for high-priority conversion points like "Download APK."

### Cards
- Surfaces should use the `Cream` color or a very light `Clay` tint.
- Borders: 1px `clay-muted`.
- Padding: 24px on desktop, 16px on mobile.

### Input Fields (Admin Portal)
- Background: `Cream` (50% opacity).
- Bottom border only or full 1px border in `clay-muted`.
- Focus state: `Amber` border.

### Chips & Tags
- Used for artifact categories (e.g., "Ceremonial," "19th Century").
- Pill-shaped, light clay background, Terracotta text.

### Artifact Display
- Always use a soft-rounded container (1rem) for artifact images.
- Backgrounds behind transparent PNG artifacts should be a subtle radial gradient of `Cream` to `Clay`.