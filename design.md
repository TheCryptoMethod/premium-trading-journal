This document outlines the core design system for the "Quantum Edge" premium trading journal, ensuring a consistent, modern, and professional user experience tailored for daytraders.

---

# Design System: Quantum Edge

## 1. Color Palette

A modern, dark color scheme designed to reduce eye strain during long trading sessions, with vibrant accents for key data and interactive elements.

*   **Background Primary:** `#0A0A0C` (Deep Charcoal - main background)
*   **Background Secondary:** `#1A1A1E` (Dark Grey - for cards, modals, distinct sections)
*   **Text Primary:** `#E0E0E0` (Soft White - main body text, headings)
*   **Text Secondary:** `#A0A0A0` (Medium Grey - secondary text, descriptions, disabled states)
*   **Primary Accent:** `#6A5ACD` (Slate Blue/Purple - for branding elements, primary buttons, active states)
*   **Secondary Accent:** `#00C896` (Vibrant Teal - for positive indicators, success states, key CTAs)
*   **Danger/Error:** `#FF6B6B` (Vibrant Red - for negative indicators, error messages)
*   **Border/Divider:** `#3A3A4A` (Darker Desaturated Purple/Grey)

## 2. Typography

Using a single, highly legible sans-serif font for consistency and a modern feel.

*   **Font Family:** `Inter` (Google Fonts)
*   **Font Weights:** Regular (400), Medium (500), SemiBold (600), Bold (700)
*   **Line Height:**
    *   Headings: 1.2
    *   Body Text: 1.6

### Font Sizes (px)

| Element       | Desktop (>=1024px) | Tablet (768px-1023px) | Mobile (<=767px) |
| :------------ | :----------------- | :-------------------- | :--------------- |
| **H1**        | 64px (Bold)        | 48px (Bold)           | 36px (Bold)      |
| **H2**        | 48px (Bold)        | 36px (Bold)           | 28px (Bold)      |
| **H3**        | 32px (SemiBold)    | 28px (SemiBold)       | 24px (SemiBold)  |
| **H4**        | 24px (SemiBold)    | 20px (SemiBold)       | 18px (SemiBold)  |
| **Body Large**| 18px (Regular)     | 16px (Regular)        | 16px (Regular)   |
| **Body Regular**| 16px (Regular)   | 15px (Regular)        | 14px (Regular)   |
| **Body Small**| 14px (Regular)     | 13px (Regular)        | 12px (Regular)   |
| **Caption**   | 12px (Regular)     | 12px (Regular)        | 11px (Regular)   |

## 3. Spacing Scale

A consistent 8px base grid for all spacing, ensuring visual harmony.

*   `--spacing-xs`: 8px
*   `--spacing-sm`: 16px
*   `--spacing-md`: 24px
*   `--spacing-lg`: 32px
*   `--spacing-xl`: 48px
*   `--spacing-xxl`: 64px
*   `--spacing-xxxl`: 96px

## 4. Border Radius

Subtle rounding for a modern, soft aesthetic.

*   `--radius-none`: 0px
*   `--radius-sm`: 4px
*   `--radius-md`: 8px
*   `--radius-lg`: 12px
*   `--radius-full`: 9999px (for pills, avatars)

## 5. Shadow Styles

Subtle, dark shadows to create depth without being distracting in a dark theme.

*   `--shadow-sm`: `0px 2px 4px rgba(0, 0, 0, 0.2)`
*   `--shadow-md`: `0px 4px 8px rgba(0, 0, 0, 0.3)`
*   `--shadow-lg`: `0px 8px 16px rgba(0, 0, 0, 0.4)`
*   `--shadow-xl`: `0px 12px 24px rgba(0, 0, 0, 0.5)`

## 6. Component Specifications by Section

### Hero Section

*   **Layout:** Full-width, vertically and horizontally centered content.
*   **Background:** `--background-primary` with a subtle, abstract geometric pattern or a blurred, low-opacity image of trading charts/data.
*   **Heading (H1):** Bold, `Inter`, `--text-primary`. Key phrases related to "trading edge" or "performance" should use `--secondary-accent`.
*   **Sub-heading (Body Large):** `Inter`, `--text-primary`, slightly lighter weight.
*   **Call to Action (CTA) Button:** Prominent, `--secondary-accent` background, `--text-primary` text. `--radius-md`. Hover effect: slight scale up, background darkens slightly.
*   **Secondary CTA (optional):** Outline button, `--primary-accent` border, `--text-primary` text.
*   **Visual Element:** A clean, modern mockup of the journal interface (e.g., a dashboard screenshot) displayed on a dark device, possibly with subtle animation or data visualization.

### Features Section

*   **Layout:** Grid-based. Desktop: 3 columns. Tablet: 2 columns. Mobile: 1 column.
*   **Feature Cards:**
    *   **Background:** `--background-secondary`.
    *   **Border Radius:** `--radius-lg`.
    *   **Shadow:** `--shadow-md` on hover.
    *   **Icon:** Prominent, clean SVG icons in `--secondary-accent` color.
    *   **Heading (H3/H4):** `Inter`, `--text-primary`.
    *   **Description (Body Regular):** `Inter`, `--text-secondary`.
    *   **Visuals:** Small, clean screenshots or abstract data visualizations can be embedded within cards, or a larger hero image for the section.

### Pricing Section

*   **Layout:** Centered, 3-column layout for pricing tiers on desktop. Stacked on tablet/mobile.
*   **Pricing Cards:**
    *   **Background:** `--background-secondary` for standard tiers. The "Most Popular" tier should have a `--primary-accent` background.
    *   **Border Radius:** `--radius-lg`.
    *   **Shadow:** `--shadow-lg` for the "Most Popular" card, `--shadow-md` for others.
    *   **Tier Name (H3):** `Inter`, `--text-primary`.
    *   **Price (H1/H2):** Large, bold, `--secondary-accent` color.
    *   **Billing Cycle (Body Small):** `--text-secondary`.
    *   **Feature List:** Bullet points, `--text-primary`, with checkmark icons in `--secondary-accent` color.
    *   **Call to Action (CTA) Button:** `--secondary-accent` background, `--text-primary` text. Full width within card.

### Footer Section

*   **Layout:** Dark background, multiple columns for navigation links (e.g., Company, Product, Resources, Legal).
*   **Background:** `--background-primary`.
*   **Text:** `--text-primary` for main text, `--text-secondary` for copyright.
*   **Links:** `--text-primary` color. Hover state changes to `--primary-accent`.
*   **Logo:** White or `--text-primary` color version of the brand logo.
*   **Social Media Icons:** `--text-primary` color. Hover state changes to `--secondary-accent`.
*   **Copyright:** `Body Small`, `--text-secondary`.

## 7. Responsive Breakpoints

Standard breakpoints for adaptive layouts.

*   `--breakpoint-mobile`: Max 767px
*   `--breakpoint-tablet`: 768px - 1023px
*   `--breakpoint-desktop`: 1024px and up

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting or slowing down performance.

*   **Purpose:** Provide feedback, guide attention, smooth transitions.
*   **Type:**
    *   **Fades:** For showing/hiding elements (modals, tooltips, notifications). `opacity` transitions.
    *   **Subtle Transforms:** Slight `scale` (buttons on hover, interactive cards), `translateY` (elements sliding in on scroll, subtle lift on hover).
    *   **Color Transitions:** Smooth changes for button hovers, link hovers, active states.
*   **Duration:**
    *   `--animation-duration-fast`: 150ms (e.g., button hover, small state changes)
    *   `--animation-duration-normal`: 300ms (e.g., modal open/close, section transitions)
    *   `--animation-duration-slow`: 500ms (e.g., complex element reveals, page transitions)
*   **Easing:** `ease-in-out` for most general animations. `ease-out` for elements appearing.
*   **Avoid:** Bouncy, overly complex, or excessively long animations. Prioritize performance and a professional feel.