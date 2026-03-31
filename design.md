This `design.md` file outlines the core visual and interactive guidelines for the premium trading journal web application. It serves as a single source of truth for design decisions, ensuring consistency and a high-quality user experience.

---

# Design System: Premium Trading Journal

**Project:** A premium trading journal web application designed for daytraders, featuring advanced analytics and performance tracking.
**Type:** SaaS
**Style:** Dark
**Color Scheme:** Dark

---

## 1. Color Palette

A sophisticated dark theme with a vibrant accent for key interactions and data highlights.

*   **Background**: `#121212` (Deep Charcoal - Main page background)
*   **Surface/Card Background**: `#1E1E1E` (Slightly lighter charcoal - For elevated components like cards, modals)
*   **Primary Accent**: `#00C4B4` (Vibrant Teal - For CTAs, active states, key data points, primary branding)
*   **Secondary Accent**: `#6C7B95` (Muted Blue-Grey - For subtle highlights, secondary actions, borders, inactive states)
*   **Text Primary**: `#E0E0E0` (Light Grey - For main headings and body text)
*   **Text Secondary**: `#A0A0A0` (Medium Grey - For descriptions, helper text, less prominent information)
*   **Text Disabled**: `#555555` (Darker Grey - For disabled elements)
*   **Border**: `#333333` (Subtle dark border for separation)
*   **Error**: `#FF6B6B` (Red - For error messages and destructive actions)
*   **Success**: `#4CAF50` (Green - For success messages and positive indicators)
*   **Warning**: `#FFD700` (Gold - For warning messages)

---

## 2. Typography

A clean, modern, and highly readable font family for optimal data consumption and UI clarity.

*   **Font Family**: `Inter`, sans-serif (Google Fonts: `https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap`)
*   **Base Font Size**: `16px`

### Font Weights:
*   Light: `300`
*   Regular: `400`
*   Medium: `500`
*   Semi-Bold: `600`
*   Bold: `700`

### Text Styles:

*   **H1**:
    *   Font Size: `48px`
    *   Line Height: `1.2`
    *   Font Weight: `700` (Bold)
    *   Color: `var(--text-primary)`
*   **H2**:
    *   Font Size: `36px`
    *   Line Height: `1.25`
    *   Font Weight: `700` (Bold)
    *   Color: `var(--text-primary)`
*   **H3**:
    *   Font Size: `28px`
    *   Line Height: `1.3`
    *   Font Weight: `600` (Semi-Bold)
    *   Color: `var(--text-primary)`
*   **H4**:
    *   Font Size: `22px`
    *   Line Height: `1.4`
    *   Font Weight: `600` (Semi-Bold)
    *   Color: `var(--text-primary)`
*   **Body Large**:
    *   Font Size: `18px`
    *   Line Height: `1.5`
    *   Font Weight: `400` (Regular)
    *   Color: `var(--text-primary)`
*   **Body Regular**:
    *   Font Size: `16px`
    *   Line Height: `1.6`
    *   Font Weight: `400` (Regular)
    *   Color: `var(--text-primary)`
*   **Body Small**:
    *   Font Size: `14px`
    *   Line Height: `1.6`
    *   Font Weight: `400` (Regular)
    *   Color: `var(--text-secondary)`
*   **Caption**:
    *   Font Size: `12px`
    *   Line Height: `1.6`
    *   Font Weight: `400` (Regular)
    *   Color: `var(--text-secondary)`
*   **Button Text**:
    *   Font Size: `16px`
    *   Line Height: `1`
    *   Font Weight: `600` (Semi-Bold)
    *   Color: `var(--text-primary)` (or contrasting for accent buttons)

---

## 3. Spacing Scale

A consistent 8px grid system for all spacing and sizing.

*   **xs**: `4px`
*   **sm**: `8px`
*   **md**: `16px`
*   **lg**: `32px`
*   **xl**: `64px`
*   **xxl**: `128px`

---

## 4. Border Radius

Subtle rounding for a modern and friendly, yet professional, aesthetic.

*   **sm**: `4px` (For small elements like buttons, input fields)
*   **md**: `8px` (For cards, larger components)
*   **lg**: `12px` (For modals, larger containers)
*   **full**: `9999px` (For pill-shaped elements like tags, avatars)

---

## 5. Shadow Styles

Subtle shadows to provide depth and hierarchy on a dark background, avoiding harsh contrasts.

*   **elevation-1 (Subtle Lift)**:
    *   `0px 2px 4px rgba(0, 0, 0, 0.2)`
    *   *Use case:* Default state for cards, subtle separation.
*   **elevation-2 (Moderate Lift)**:
    *   `0px 4px 8px rgba(0, 0, 0, 0.3)`
    *   *Use case:* Hover state for cards, dropdowns, tooltips.
*   **elevation-3 (Prominent Lift)**:
    *   `0px 8px 16px rgba(0, 0, 0, 0.4)`
    *   *Use case:* Modals, prominent floating elements.
*   **inner-shadow (Input Fields)**:
    *   `inset 0px 1px 3px rgba(0, 0, 0, 0.5)`
    *   *Use case:* Giving depth to input fields on a dark background.

---

## 6. Component Specifications

Detailed guidelines for key sections of the application.

### 6.1. Hero Section

*   **Purpose**: Captivate users and clearly communicate the value proposition.
*   **Layout**: Centered content, full-width background.
*   **Background**: `var(--background)`
*   **Content**:
    *   **Title**:
        *   Text: "Unlock Your Trading Edge with Advanced Analytics."
        *   Style: `H1`, `var(--text-primary)`
        *   Alignment: Centered
    *   **Subtitle**:
        *   Text: "Seamlessly track performance, identify patterns, and optimize strategies with our premium trading journal."
        *   Style: `Body Large`, `var(--text-secondary)`
        *   Alignment: Centered
        *   Max Width: `700px`
    *   **Call to Action (CTA) Button**:
        *   Text: "Start Your Free Trial"
        *   Background: `var(--primary-accent)`
        *   Text Color: `var(--text-primary)` (or a slightly darker contrasting color if needed for accessibility on teal)
        *   Padding: `14px 32px`
        *   Border Radius: `var(--border-radius-sm)`
        *   Hover: Slight background darken, `elevation-1` shadow.
    *   **Visual Element**:
        *   Concept: Abstract data visualization, stylized stock charts, or a sleek illustration of the app UI on a dark, premium device.
        *   Placement: Below text content, or subtly integrated into the background.

### 6.2. Features Section

*   **Purpose**: Highlight key functionalities and benefits.
*   **Layout**: Grid of feature cards, centered section title.
*   **Background**: `var(--background)`
*   **Content**:
    *   **Section Title**:
        *   Text: "Powerful Features to Elevate Your Trading"
        *   Style: `H2`, `var(--text-primary)`
        *   Alignment: Centered
    *   **Feature Cards (Grid)**:
        *   **Card Background**: `var(--surface-card-background)`
        *   **Card Padding**: `var(--lg)`
        *   **Border Radius**: `var(--border-radius-md)`
        *   **Shadow**: `var(--elevation-1)` (on hover: `var(--elevation-2)`)
        *   **Icon**:
            *   Style: SVG, `24px` or `32px` size.
            *   Color: `var(--primary-accent)`
        *   **Feature Title**:
            *   Style: `H4`, `var(--text-primary)`
        *   **Feature Description**:
            *   Style: `Body Regular`, `var(--text-secondary)`
        *   **Example Features**:
            *   "Advanced Performance Metrics": Detailed analytics on trades.
            *   "Customizable Journal Entries": Flexible logging for every trade.
            *   "Strategy Backtesting": Test strategies against historical data.
            *   "Interactive Charting": Visualize trades directly on charts.
            *   "Risk Management Tools": Built-in tools to manage exposure.
            *   "Multi-Broker Integration": Connect with various trading platforms.

### 6.3. Pricing Section

*   **Purpose**: Present subscription plans clearly and encourage conversion.
*   **Layout**: Grid of pricing cards, centered section title.
*   **Background**: `var(--background)`
*   **Content**:
    *   **Section Title**:
        *   Text: "Simple, Transparent Pricing"
        *   Style: `H2`, `var(--text-primary)`
        *   Alignment: Centered
    *   **Pricing Cards (Grid)**:
        *   **Card Background**: `var(--surface-card-background)`
        *   **Card Padding**: `var(--lg)`
        *   **Border Radius**: `var(--border-radius-md)`
        *   **Shadow**: `var(--elevation-1)` (highlighted plan: `var(--elevation-2)`)
        *   **Plan Name**:
            *   Style: `H3`, `var(--text-primary)`
        *   **Price**:
            *   Style: `H1` (adjusted to `40px` for pricing), `var(--text-primary)`
            *   Suffix: `/month` or `/year` (Body Small, `var(--text-secondary)`)
        *   **Features List**:
            *   Style: `Body Regular`, `var(--text-primary)`
            *   Each feature preceded by a checkmark icon (`var(--primary-accent)`)
        *   **Call to Action (CTA) Button**:
            *   Text: "Choose Plan"
            *   Background: `var(--primary-accent)`
            *   Text Color: `var(--text-primary)`
            *   Padding: `12px 24px`
            *   Border Radius: `var(--border-radius-sm)`
            *   Hover: Slight background darken, `elevation-1` shadow.
        *   **Example Plans**: "Basic Trader", "Pro Analyst", "Elite Strategist"

### 6.4. Footer Section

*   **Purpose**: Provide essential links and copyright information.
*   **Layout**: Full-width, divided into columns or rows for links and copyright.
*   **Background**: `var(--background)` (or slightly darker if desired, e.g., `#0A0A0A`)
*   **Content**:
    *   **Copyright**:
        *   Text: "© 2023 [Project Name]. All rights reserved."
        *   Style: `Caption`, `var(--text-secondary)`
    *   **Navigation Links**:
        *   Links: "Privacy Policy", "Terms of Service", "Support", "About Us"
        *   Style: `Body Small`, `var(--text-secondary)`
        *   Hover: `var(--primary-accent)`
    *   **Social Media Links**:
        *   Icons: Twitter, LinkedIn, etc. (SVG)
        *   Style: `20px` size, `var(--text-secondary)`
        *   Hover: `var(--primary-accent)`

---

## 7. Responsive Breakpoints

Standard breakpoints for adapting the layout across devices.

*   **Mobile**: `< 768px` (e.g., `max-width: 767px`)
*   **Tablet**: `768px - 1023px` (e.g., `min-width: 768px` and `max-width: 1023px`)
*   **Desktop**: `1024px +` (e.g., `min-width: 1024px`)

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Purpose**: Provide visual feedback, guide user attention, and add a premium feel.
*   **Duration**:
    *   Short (e.g., hover states, small changes): `150ms - 200ms`
    *   Medium (e.g., modal transitions, section fades): `250ms - 350ms`
*   **Easing**:
    *   Most transitions: `ease-in-out` (smooth start and end)
    *   Quick feedback: `ease-out`
*   **Common Animations**:
    *   **Hover Effects**: Buttons, links, and cards should have subtle visual feedback (e.g., slight background color change, `elevation-1` shadow, minor scale).
    *   **State Changes**: Input fields, checkboxes, and toggles should animate smoothly between states.
    *   **Modals/Drawers**: Fade in/out with a slight scale or slide effect.
    *   **Data Updates**: Subtle fade or slide for new data appearing in charts or tables.
    *   **Scroll Reveal**: Elements fading or sliding into view as the user scrolls, but used sparingly to avoid overuse.

---