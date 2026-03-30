# Design System Documentation: Premium Trading Journal

This document outlines the core design principles and specifications for the Premium Trading Journal SaaS project. It serves as a single source of truth for all UI/UX elements, ensuring consistency and efficiency in development.

---

## 1. Project Overview

*   **Project Name:** Premium Trading Journal
*   **Type:** SaaS (Software as a Service)
*   **Description:** A sophisticated trading journal for Futures and Crypto Daytraders, providing advanced analytics, performance tracking, backtesting, and equity curve visualization.
*   **Style:** Dark, professional, modern, data-focused.

---

## 2. Color Palette

The color palette is designed to be dark, professional, and easy on the eyes during long trading sessions, with clear indicators for performance metrics.

*   **Background:**
    *   `--color-background-primary`: `#0A0A0C` (Deepest dark grey, almost black)
    *   `--color-background-secondary`: `#1A1A1D` (Slightly lighter dark grey for cards/sections)
    *   `--color-background-tertiary`: `#2C2C30` (For elevated elements like modals, tooltips)
*   **Primary Brand Colors:**
    *   `--color-primary`: `#6C63FF` (Deep professional purple for main branding, active states)
    *   `--color-primary-light`: `#8E88FF` (Lighter purple for secondary actions, subtle highlights)
*   **Accent Color:**
    *   `--color-accent`: `#00C896` (Vibrant teal/green for CTAs, profit indicators, key data points)
*   **Text Colors:**
    *   `--color-text-primary`: `#E0E0E0` (Light grey for main content)
    *   `--color-text-secondary`: `#A0A0A0` (Medium grey for secondary information, labels)
    *   `--color-text-tertiary`: `#6B6B6B` (Darker grey for subtle details, timestamps)
*   **Status Colors:**
    *   `--color-success`: `#00C896` (Profit, positive indicators - same as accent)
    *   `--color-error`: `#FF4D4D` (Loss, negative indicators, error messages)
    *   `--color-warning`: `#FFC107` (Caution, alerts)
    *   `--color-info`: `#5BC0DE` (Informational messages)
*   **Border Colors:**
    *   `--color-border-light`: `#3A3A3F` (Light border for subtle separation)
    *   `--color-border-dark`: `#252528` (Darker border for internal component separation)

---

## 3. Typography

The `Inter` font family is chosen for its modern, clean, and highly readable characteristics across various sizes and weights, suitable for data-intensive applications.

*   **Font Family:**
    *   `--font-family-headings`: `'Inter', sans-serif`
    *   `--font-family-body`: `'Inter', sans-serif`
*   **Font Weights:**
    *   `--font-weight-light`: 300
    *   `--font-weight-regular`: 400
    *   `--font-weight-medium`: 500
    *   `--font-weight-semibold`: 600
    *   `--font-weight-bold`: 700
*   **Font Sizes (Responsive):**
    *   **H1 (Page Title/Hero Headline):**
        *   Desktop: `64px` (`--font-size-h1-desktop`)
        *   Tablet: `48px` (`--font-size-h1-tablet`)
        *   Mobile: `36px` (`--font-size-h1-mobile`)
        *   Line Height: `1.2`
        *   Weight: `bold`
    *   **H2 (Section Titles):**
        *   Desktop: `48px` (`--font-size-h2-desktop`)
        *   Tablet: `36px` (`--font-size-h2-tablet`)
        *   Mobile: `28px` (`--font-size-h2-mobile`)
        *   Line Height: `1.3`
        *   Weight: `semibold`
    *   **H3 (Card Titles, Sub-sections):**
        *   Desktop: `32px` (`--font-size-h3-desktop`)
        *   Tablet: `28px` (`--font-size-h3-tablet`)
        *   Mobile: `24px` (`--font-size-h3-mobile`)
        *   Line Height: `1.4`
        *   Weight: `semibold`
    *   **H4 (Component Titles, FAQ Questions):**
        *   Desktop: `24px` (`--font-size-h4-desktop`)
        *   Tablet: `20px` (`--font-size-h4-tablet`)
        *   Mobile: `18px` (`--font-size-h4-mobile`)
        *   Line Height: `1.5`
        *   Weight: `medium`
    *   **Body Large (Lead paragraphs, important text):**
        *   All devices: `18px` (`--font-size-body-lg`)
        *   Line Height: `1.6`
        *   Weight: `regular`
    *   **Body (Standard text):**
        *   All devices: `16px` (`--font-size-body`)
        *   Line Height: `1.6`
        *   Weight: `regular`
    *   **Body Small (Metadata, captions, legal text):**
        *   All devices: `14px` (`--font-size-body-sm`)
        *   Line Height: `1.6`
        *   Weight: `regular`
    *   **Caption (Smallest text, e.g., chart labels):**
        *   All devices: `12px` (`--font-size-caption`)
        *   Line Height: `1.5`
        *   Weight: `regular`

---

## 4. Spacing Scale

A consistent 8px base spacing scale is used to maintain rhythm and hierarchy.

*   `--spacing-xs`: `4px`
*   `--spacing-sm`: `8px`
*   `--spacing-md`: `16px`
*   `--spacing-lg`: `24px`
*   `--spacing-xl`: `32px`
*   `--spacing-2xl`: `48px`
*   `--spacing-3xl`: `64px`
*   `--spacing-4xl`: `96px`
*   `--spacing-5xl`: `128px`

---

## 5. Border Radius

Subtle rounding for a modern, friendly, yet professional feel.

*   `--border-radius-none`: `0px`
*   `--border-radius-sm`: `4px`
*   `--border-radius-md`: `8px`
*   `--border-radius-lg`: `12px`
*   `--border-radius-full`: `9999px` (For pill-shaped elements like buttons, tags)

---

## 6. Shadow Styles

Shadows are used sparingly and subtly to provide depth and emphasize interactive elements, especially on a dark background where strong shadows can be lost. Focus on inner glows or very soft, low-opacity outer shadows.

*   `--shadow-sm`: `0px 1px 3px rgba(0, 0, 0, 0.2), 0px 1px 2px rgba(0, 0, 0, 0.12)`
*   `--shadow-md`: `0px 4px 6px rgba(0, 0, 0, 0.3), 0px 2px 4px rgba(0, 0, 0, 0.18)`
*   `--shadow-lg`: `0px 10px 15px rgba(0, 0, 0, 0.4), 0px 4px 6px rgba(0, 0, 0, 0.24)`
*   `--shadow-card-hover`: `0px 0px 0px 2px var(--color-primary) inset` (Subtle inner glow for interactive cards/elements on hover)
*   `--shadow-button-focus`: `0px 0px 0px 3px rgba(108, 99, 255, 0.5)` (Focus ring for accessibility)

---

## 7. Component Specifications by Section

### 7.1. Hero Section

*   **Layout:** Full-width, centered content. Left-aligned text, right-aligned image/mockup on desktop. Stacked on mobile.
*   **Background:** `--color-background-primary`
*   **Headline:**
    *   Text: "Unlock Your Trading Edge with Advanced Analytics."
    *   Style: `H1`, `--font-weight-bold`, `--color-text-primary`
*   **Subheadline:**
    *   Text: "Seamlessly track P&L, win-rate, entry/exit timing, and backtest strategies for Futures and Crypto Daytraders."
    *   Style: `Body Large`, `--color-text-secondary`
*   **Call to Action (CTA) Button:**
    *   Text: "Start Free Trial"
    *   Background: `--color-accent`
    *   Text Color: `--color-background-primary` (or pure white `#FFFFFF` for contrast)
    *   Border Radius: `--border-radius-md`
    *   Padding: `--spacing-md` vertical, `--spacing-xl` horizontal
    *   Hover: `background-color` darkens slightly, `--shadow-button-focus`
*   **Secondary CTA (Optional):**
    *   Text: "Learn More"
    *   Background: Transparent
    *   Text Color: `--color-primary`
    *   Border: `1px solid var(--color-primary)`
    *   Border Radius: `--border-radius-md`
    *   Padding: `--spacing-md` vertical, `--spacing-xl` horizontal
    *   Hover: `background-color` `rgba(108, 99, 255, 0.1)`
*   **Image/Video:** High-quality mockup of the journal UI, showcasing key features in a dark theme.

### 7.2. Features Section

*   **Layout:** Grid-based, 3 columns on desktop, 2 columns on tablet, 1 column on mobile.
*   **Background:** `--color-background-secondary`
*   **Section Title:**
    *   Text: "Powerful Features Designed for Traders"
    *   Style: `H2`, `--font-weight-semibold`, `--color-text-primary`
*   **Feature Card:**
    *   **Container:**
        *   Background: `--color-background-tertiary`
        *   Border Radius: `--border-radius-lg`
        *   Padding: `--spacing-xl`
        *   Shadow: `--shadow-sm`
        *   Hover: `--shadow-card-hover`
    *   **Icon:**
        *   Size: `48px x 48px`
        *   Color: `--color-primary`
        *   Background: `rgba(108, 99, 255, 0.1)` (subtle circle)
        *   Border Radius: `50%`
    *   **Title:**
        *   Style: `H4`, `--font-weight-medium`, `--color-text-primary`
        *   Margin Top: `--spacing-md`
    *   **Description:**
        *   Style: `Body`, `--color-text-secondary`
        *   Margin Top: `--spacing-sm`

### 7.3. Pricing Section

*   **Layout:** Centered content. Pricing cards arranged in a row (3 columns desktop, 2 tablet, 1 mobile).
*   **Background:** `--color-background-primary`
*   **Section Title:**
    *   Text: "Simple, Transparent Pricing"
    *   Style: `H2`, `--font-weight-semibold`, `--color-text-primary`
*   **Pricing Toggle (Monthly/Annually):**
    *   Style: Pill-shaped toggle with active state highlighted by `--color-primary`.
    *   Text Color: `--color-text-secondary` (inactive), `--color-text-primary` (active)
*   **Pricing Card:**
    *   **Container:**
        *   Background: `--color-background-secondary`
        *   Border Radius: `--border-radius-lg`
        *   Padding: `--spacing-2xl`
        *   Shadow: `--shadow-md`
        *   Highlighted Plan (e.g., "Pro"): `border: 2px solid var(--color-primary)`
    *   **Plan Name:**
        *   Style: `H3`, `--font-weight-semibold`, `--color-text-primary`
    *   **Price:**
        *   Large, bold text (e.g., `H1` size, `--font-weight-bold`)
        *   Currency symbol: `--color-text-secondary`
        *   Number: `--color-text-primary`
        *   Per period: `Body Small`, `--color-text-secondary`
    *   **Features List:**
        *   List items: `Body`, `--color-text-primary`
        *   Checkmark icon: `--color-success`
        *   Spacing: `--spacing-sm` between items
    *   **CTA Button:**
        *   Text: "Choose Plan"
        *   Background: `--color-primary` (for standard), `--color-accent` (for highlighted plan)
        *   Text Color: `--color-background-primary`
        *   Border Radius: `--border-radius-md`
        *   Padding: `--spacing-md` vertical, `--spacing-xl` horizontal
        *   Hover: `background-color` darkens slightly, `--shadow-button-focus`

### 7.4. FAQ Section

*   **Layout:** Centered content, max-width container.
*   **Background:** `--color-background-secondary`
*   **Section Title:**
    *   Text: "Frequently Asked Questions"
    *   Style: `H2`, `--font-weight-semibold`, `--color-text-primary`
*   **Accordion Component:**
    *   **Question Header:**
        *   Background: `--color-background-tertiary`
        *   Padding: `--spacing-lg`
        *   Border Radius: `--border-radius-md`
        *   Text: `H4`, `--font-weight-medium`, `--color-text-primary`
        *   Icon: Chevron icon, rotates on open/close.
        *   Hover: `background-color` slightly lighter `var(--color-background-tertiary)`
    *   **Answer Content:**
        *   Background: `--color-background-tertiary` (or transparent if preferred)
        *   Padding: `--spacing-lg` (top/bottom), `--spacing-xl` (left/right)
        *   Text: `Body`, `--color-text-secondary`
        *   Transition: Smooth slide/fade on open/close.

### 7.5. Footer Section

*   **Layout:** Full-width, multi-column on desktop (e.g., Logo/Description, Navigation, Social, Legal). Stacked on mobile.
*   **Background:** `--color-background-primary`
*   **Logo:** SVG or high-res PNG, white/light version.
*   **Description:**
    *   Text: Brief project description.
    *   Style: `Body Small`, `--color-text-secondary`
*   **Navigation Links:**
    *   Text: `Body Small`, `--color-text-secondary`
    *   Hover: `color: var(--color-primary)`
*   **Social Media Icons:**
    *   Icons: Standard social media icons (Twitter, Discord, etc.)
    *   Color: `--color-text-secondary`
    *   Hover: `color: var(--color-primary)`
*   **Copyright:**
    *   Text: `Body Small`, `--color-text-tertiary`
    *   Margin Top: `--spacing-xl`

---

## 8. Responsive Breakpoints

These breakpoints define how the layout and components adapt to different screen sizes.

*   **Mobile:**
    *   `--breakpoint-mobile-max`: `max-width: 767px`
    *   Target devices: Smartphones (portrait & landscape)
*   **Tablet:**
    *   `--breakpoint-tablet-min`: `min-width: 768px`
    *   `--breakpoint-tablet-max`: `max-width: 1023px`
    *   Target devices: Tablets (portrait & landscape), small laptops
*   **Desktop:**
    *   `--breakpoint-desktop-min`: `min-width: 1024px`
    *   `--breakpoint-desktop-max`: `max-width: 1439px`
    *   Target devices: Standard laptops, desktop monitors
*   **Large Desktop:**
    *   `--breakpoint-large-desktop-min`: `min-width: 1440px`
    *   Target devices: Large monitors, ultra-wide screens

---

## 9. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting. They should feel fast and fluid.

*   **Duration:**
    *   `--animation-duration-fast`: `150ms` (for hover states, small changes)
    *   `--animation-duration-normal`: `250ms` (for modal transitions, accordion toggles)
    *   `--animation-duration-slow`: `350ms` (for complex transitions, page loads)
*   **Easing:**
    *   `--animation-easing-ease-in-out`: `cubic-bezier(0.4, 0, 0.2, 1)` (Standard smooth curve)
    *   `--animation-easing-ease-out`: `cubic-bezier(0, 0, 0.2, 1)` (Starts fast, ends slow)
*   **Types of Animations:**
    *   **Hover States:** Subtle `background-color` changes, `border-color` changes, `transform: translateY(-2px)` for elevation.
    *   **Focus States:** Clear `box-shadow` or `outline` for accessibility.
    *   **Transitions:** `opacity` for fades, `transform: translateX/Y` for slides, `height` for accordion open/close.
    *   **Loading States:** Subtle spinners or skeleton loaders.
    *   **Modals/Drawers:** Fade in/out with slight scale or slide.
*   **Principles:**
    *   **Purposeful:** Every animation should serve a clear UX purpose (feedback, hierarchy, context).
    *   **Performant:** Avoid animations that cause jank or slow down the interface. Use `transform` and `opacity` where possible for hardware acceleration.
    *   **Subtle:** No flashy or overly complex animations.
    *   **Consistent:** Apply similar animation styles to similar interactions across the platform.