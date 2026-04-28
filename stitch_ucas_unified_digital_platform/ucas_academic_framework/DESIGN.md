---
name: UCAS Academic Framework
colors:
  surface: '#faf8ff'
  surface-dim: '#dad9e1'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3fa'
  surface-container: '#eeedf4'
  surface-container-high: '#e9e7ef'
  surface-container-highest: '#e3e1e9'
  on-surface: '#1a1b21'
  on-surface-variant: '#444651'
  inverse-surface: '#2f3036'
  inverse-on-surface: '#f1f0f7'
  outline: '#757682'
  outline-variant: '#c5c5d3'
  surface-tint: '#4059aa'
  primary: '#00236f'
  on-primary: '#ffffff'
  primary-container: '#1e3a8a'
  on-primary-container: '#90a8ff'
  inverse-primary: '#b6c4ff'
  secondary: '#00687a'
  on-secondary: '#ffffff'
  secondary-container: '#57dffe'
  on-secondary-container: '#006172'
  tertiary: '#4b1c00'
  on-tertiary: '#ffffff'
  tertiary-container: '#6e2c00'
  on-tertiary-container: '#f39461'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b6c4ff'
  on-primary-fixed: '#00164e'
  on-primary-fixed-variant: '#264191'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#ffdbcb'
  tertiary-fixed-dim: '#ffb691'
  on-tertiary-fixed: '#341100'
  on-tertiary-fixed-variant: '#773205'
  background: '#faf8ff'
  on-background: '#1a1b21'
  surface-variant: '#e3e1e9'
typography:
  h1:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.25'
  h3:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Work Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Work Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Work Sans
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.01em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 48px
  xl: 64px
  container-max: 1280px
---

## Brand & Style

The design system is rooted in the "Academic Modernism" style, prioritizing clarity, authority, and accessibility for the University College of Applied Sciences. The brand personality is institutional yet progressive, balancing the tradition of deep academia with the agility of applied sciences. 

The aesthetic leverages a minimalist framework characterized by expansive whitespace, a restrained color palette, and high-contrast elements to ensure legibility for a diverse student and faculty population. Visual hierarchy is established through precise typographic scales and subtle depth rather than decorative elements. The system must feel equally native in both English (LTR) and Arabic (RTL) contexts, ensuring structural integrity and optical balance across scripts.

## Colors

The palette is anchored by **Deep Blue (#1E3A8A)**, representing stability and academic excellence. **Teal/Cyan (#06B6D4)** serves as the secondary accent, used sparingly for interaction cues, progress indicators, and digital-first highlights. 

The neutral palette utilizes a range of cool grays to maintain a clean, "paper-like" feel. Backgrounds should predominantly use the neutral light gray or pure white to maximize contrast. For accessibility, all primary actions must maintain a contrast ratio of at least 4.5:1 against their backgrounds. In RTL contexts, color application remains consistent, ensuring that semantic colors (like success green or error red) are mirrored in their logical placement.

## Typography

This design system uses a dual-font strategy to differentiate between structural headings and long-form content. **Plus Jakarta Sans** (serving as the geometric alternative to Poppins) provides a modern, bold presence for headings, ensuring the institution feels contemporary. **Work Sans** (serving as the highly legible alternative to Roboto) is used for all body copy and UI labels, optimized for screen readability and high information density.

For Arabic support, use a system font stack that matches the weight and optical sizing of the Latin counterparts (e.g., IBM Plex Sans Arabic or Noto Sans Arabic). Ensure line-heights are increased by approximately 20% for Arabic text to prevent diacritic clipping.

## Layout & Spacing

The layout is built on a strict 8px grid system. For desktop, a 12-column fluid grid is used with 24px gutters. On mobile devices, a 4-column grid with 16px margins is standard. 

Spacing follows a logical progression where related elements (like a label and an input) use `xs` (8px), while distinct sections use `lg` (48px) to provide "breathing room." In RTL mode, all horizontal spacing, margins, and paddings must be flipped (e.g., `padding-left` becomes `padding-right`). Use logical properties (`padding-inline-start`) in CSS to handle this automatically.

## Elevation & Depth

Depth is conveyed through "Ambient Shadows"—soft, diffused, and low-opacity. This design system avoids heavy drop shadows to maintain a minimalist profile. 

- **Level 0 (Flat):** Used for the main background.
- **Level 1 (Raised):** Cards and Input fields. Uses a 4px blur with 5% opacity of the Primary Deep Blue color to create a "tinted" shadow.
- **Level 2 (Floating):** Navigation bars and Toast notifications. Uses a 12px blur with 10% opacity.

The goal is to suggest that elements are resting slightly above the surface rather than flying high. High-contrast outlines (1px width in light gray) are used in conjunction with shadows to define boundaries clearly for users with visual impairments.

## Shapes

The shape language is "Rounded," utilizing a 0.5rem (8px) base radius for standard components like buttons and inputs. Larger containers, such as cards and toast notifications, use a 1rem (16px) radius. This softening of corners balances the "hard" professional blue and bold typography, making the digital experience feel more approachable and less rigid. Icons should follow a similar language, utilizing rounded terminals and consistent stroke weights.

## Components

### Buttons
- **Primary:** Solid Deep Blue background with white text. High-contrast, bold weight.
- **Secondary:** Outlined with a 2px Teal border and Teal text. Clear interactive state changes (slight background fill on hover).

### Input Fields
- Height of 48px for touch-friendliness. 
- 1px light gray border that transitions to Deep Blue on focus. 
- Labels are always visible (not floating) to aid cognitive load for students.

### Cards
- Used for course modules or news.
- White background with a Level 1 shadow and 16px rounded corners.
- Padding should be a minimum of 24px (md).

### Navigation Bar (Mobile)
- Bottom-docked for reachability.
- Features clear labels under icons. 
- Uses a background blur (Glassmorphism effect) with a white tint to stay legible over content.

### Toast Notifications
- Positioned at the top-center on mobile.
- Utilizes the Secondary Teal for informational alerts and Deep Blue for branding. 
- Includes a 1px border to ensure visibility against varied content.

### RTL Considerations
For all components, the "Start" and "End" logic applies. Icons that indicate direction (like "Back" or "Next" arrows) must be mirrored in the Arabic interface. Navigation labels must be right-aligned, and the sequence of multi-step inputs must flow from right to left.