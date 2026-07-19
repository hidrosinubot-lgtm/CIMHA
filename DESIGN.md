---
name: Hydrologic Precision System
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
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#271901'
  on-tertiary-container: '#98805d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#fcdeb5'
  tertiary-fixed-dim: '#dec29a'
  on-tertiary-fixed: '#271901'
  on-tertiary-fixed-variant: '#574425'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-metric:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
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
  body-lg:
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
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-margin-mobile: 16px
  container-margin-desktop: 32px
  gutter: 16px
  stack-sm: 4px
  stack-md: 12px
  stack-lg: 24px
---

## Brand & Style

This design system is built for high-stakes environmental monitoring, where clarity and reliability are paramount. The brand personality is authoritative yet approachable, prioritizing data legibility and functional efficiency over decorative elements.

The aesthetic follows a **Corporate Minimalism** approach. It utilizes expansive whitespace to reduce cognitive load during data analysis and employs a rigorous grid system to organize complex information. The interface should feel like a precision instrument: silent, dependable, and meticulously structured. The emotional response sought is one of "calm control"—providing the user with the confidence to make critical decisions based on real-time hydrometeorological data.

## Colors

The palette is anchored by a deep, authoritative blue that evokes the depth of water and the vastness of the atmosphere. 

- **Primary:** A deep navy used for core branding, primary actions, and critical navigation elements to instill trust.
- **Secondary:** A bright, functional blue used for interactive states, data highlights, and link text.
- **Neutral/Background:** Predominantly white (`#FFFFFF`) to ensure maximum contrast and a clean workspace. Off-whites and soft grays are used for section backgrounds and surface layering to prevent eye strain.
- **Disabled/Border:** Low-saturation grays define boundaries without competing for the user's attention.

## Typography

The design system utilizes **Inter** for its exceptional legibility in technical contexts. The typographic hierarchy is designed to highlight critical metrics (water levels, precipitation rates) while maintaining a clean flow for supporting information.

- **Display Metrics:** Used specifically for the primary data point on a dashboard.
- **Headlines:** Reserved for section titles and modal headers.
- **Body Text:** Optimized for readability in reports and data descriptions.
- **Label Caps:** Used for metadata, units of measurement, and table headers to provide clear categorization without occupying significant space.

## Layout & Spacing

This design system employs an **8px linear scale** to ensure mathematical harmony across all components. 

- **Grid:** A 12-column fluid grid is used for desktop monitoring dashboards, transitioning to a single-column layout for mobile. 
- **Margins:** 16px safe areas are enforced on mobile devices, increasing to 32px on desktop to emphasize the "clean" minimalist aesthetic.
- **Rhythm:** Vertical spacing between cards and data blocks should favor generous "stack-lg" units to maintain a professional, uncluttered feel. Components within a group (like a label and its input) should use "stack-sm".

## Elevation & Depth

Visual hierarchy is achieved through **Tonal Layering** and **Subtle Shadows** rather than heavy color fills.

- **Level 0 (Base):** The primary background, usually white or the softest gray.
- **Level 1 (Cards/Surface):** Elevated by a 1px solid border in a soft gray (`#E2E8F0`). No shadow is used for standard cards to keep the UI flat and professional.
- **Level 2 (Modals/Bottom Sheets):** These elements use a soft, ambient shadow (0px 10px 25px rgba(0,0,0,0.05)) to suggest they are floating above the data layer. 
- **Scrim:** When a modal or bottom sheet is active, a 40% opacity navy scrim is applied to the background to focus the user’s attention.

## Shapes

The shape language is refined and approachable. A consistent **0.5rem (8px)** corner radius is applied to all primary containers, buttons, and input fields. 

This specific level of roundedness softens the technical nature of the data without appearing overly "bubbly" or consumer-focused. Large containers like dashboard cards may use the `rounded-lg` (1rem) variant to better frame complex data visualizations.

## Components

### Buttons
- **Primary:** Full-width on mobile, navy background, white text. High contrast for critical actions like "Generate Report."
- **Secondary/Disabled:** A soft gray background (`#F1F5F9`) with slate text. Use for "Cancel" or inactive states where data is still loading.

### Selectors & Inputs
- **Form Fields:** Defined 1px borders using the secondary gray. Focused states must use the primary blue for the border and a subtle 2px outer glow.
- **Dropdowns:** Use a chevron-down icon and clear, high-contrast labels.

### Lists & Modals
- **Ordered Lists:** Found within selection modals. Each item is separated by a 1px hair-line divider (`#F1F5F9`).
- **Bottom Sheets:** Rounded top corners (1.5rem), featuring a centered "grabber" handle at the top to indicate draggability.

### Data Visualization
- **Charts:** Use thin stroke weights (1.5pt) for line graphs to maintain the minimalist feel. Tooltips should follow the "Level 2" elevation rules with high legibility.