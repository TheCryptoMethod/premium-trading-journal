```markdown
# Design System for Premium Trading Journal

This document outlines the core design principles and specifications for the "Premium Trading Journal" SaaS project. It aims to provide a consistent and scalable foundation for UI development, ensuring a premium, professional, and intuitive user experience.

---

## 1. Color Palette

A sophisticated dark theme with vibrant accents for data visualization and interactive elements.

*   **Background Primary**: `#0A0A0C` (Deep Charcoal) - Main background for pages and sections.
*   **Background Secondary**: `#1A1A1E` (Dark Grey) - Used for cards, modals, and elevated UI elements.
*   **Text Primary**: `#E0E0E0` (Light Grey) - Main body text, labels.
*   **Text Secondary**: `#A0A0A0` (Medium Grey) - Secondary information, helper text, disabled states.
*   **Primary Accent**: `#2A64F6` (Vibrant Blue) - Main interactive elements, primary buttons, active states, key data highlights.
*   **Secondary Accent**: `#00C4B4` (Teal) - Secondary interactive elements, charts, progress indicators, positive trends.
*   **Success**: `#00E676` (Bright Green) - Positive feedback, successful actions, profit indicators.
*   **Warning**: `#FFC107` (Amber) - Cautionary messages, neutral trends.
*   **Danger**: `#DC3545` (Red) - Error messages, destructive actions, loss indicators.

---

## 2. Typography

Utilizing a modern, highly readable sans-serif font for both headings and body text to maintain consistency and clarity, crucial for data-heavy applications.

*   **Font Family**: `Inter`, `sans-serif`
    *   **Import**: `@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');`
*   **Headings Font**: `Inter`
    *   `H1`: 48px, `font-weight: 800`, `line-height: 1.2`, `color: #FFFFFF`
    *   `H2`: 36px, `font-weight: 700`, `line-height: 1.3`, `color: #FFFFFF`
    *   `H3`: 28px, `font-weight: 600`, `line-height: 1.4`, `color: #FFFFFF`
    *   `H4`: 22px, `font-weight: 600`, `line-height: 1.5`, `color: #FFFFFF`
*   **Body Font**: `Inter`
    *   `Body Large`: 18px, `font-weight: 400`, `line-height: 1.6`, `color: #E0E0E0`
    *   `Body Medium`: 16px, `font-weight: 400`, `line-height: 1.6`, `color: #E0E0E0`
    *   `Body Small`: 14px, `font-weight: 400`, `line-height: 1.7`, `color: #A0A0A0`
    *   `Caption`: 12px, `font-weight: 300`, `line-height: 1.8`, `color: #A0A0A0`
*   **Emphasis**:
    *   `Strong`: `font-weight: 600`
    *   `Link`: `color: #2A64F6`, `text-decoration: underline` on hover

---

## 3. Spacing Scale

A consistent 8px grid-based spacing system for all UI elements.

*   `xs`: 4px
*   `sm`: 8px
*   `md`: 16px
*   `lg`: 24px
*   `xl`: 32px
*   `xxl`: 48px
*   `xxxl`: 64px

---

## 4. Border Radius

Subtle rounding for a modern and friendly, yet professional aesthetic.

*   **Base Radius**: `8px` - Applied to cards, buttons, input fields, and most UI containers.
*   **Small Radius**: `4px` - For smaller elements like tags or badges.
*   **Pill Radius**: `9999px` - For pill-shaped buttons or tags.

---

## 5. Shadow Styles

Subtle shadows to provide depth and hierarchy without overwhelming the dark theme. Shadows are typically darker and less spread out than in light themes.

*   **Shadow-sm**: `0px 1px 3px rgba(0, 0, 0, 0.3)` - For subtle elevation on interactive elements.
*   **Shadow-md**: `0px 4px 8px rgba(0, 0, 0, 0.4)` - For cards, dropdowns, and modals.
*   **Shadow-lg**: `0px 10px 20px rgba(0, 0, 0, 0.5)` - For prominent modals or fixed headers/footers.
*   **Inner Shadow (for recessed elements)**: `inset 0px 1px 2px rgba(0, 0, 0, 0.6)` - For input fields or toggles.

---

## 6. Component Specifications

### 6.1. Hero Section

*   **Layout**: Full-width, centered content. Image/video on one side, text/CTA on the other (desktop). Stacked on mobile.
*   **Background**: `linear-gradient(180deg, #0A0A0C 0%, #1A1A1E 100%)` or a subtle background pattern.
*   **Headline**: `H1` (`48px`, `font-weight: 800`, `color: #FFFFFF`). Bold, impactful statement.
    *   *Example*: "Master Your Trades. Maximize Your Profits."
*   **Subheadline**: `Body Large` (`18px`, `font-weight: 400`, `color: #E0E0E0`). Clear, concise explanation.
    *   *Example*: "Advanced analytics, backtesting, and performance tracking designed for active daytraders."
*   **Call to Action (CTA)**:
    *   **Primary Button**: `background-color: #2A64F6`, `color: #FFFFFF`, `padding: 16px 32px`, `border-radius: 8px`, `font-weight: 600`, `font-size: 18px`.
        *   *Example*: "Start Free Trial"
    *   **Secondary Button (optional)**: `background-color: transparent`, `border: 1px solid #2A64F6`, `color: #2A64F6`, `padding: 16px 32px`, `border-radius: 8px`, `font-weight: 600`, `font-size: 18px`.
        *   *Example*: "Watch Demo"
*   **Visual Element**: Placeholder for a high-quality screenshot of the journal UI or a short demo video. Aspect ratio `16:9`.

### 6.2. Features Section

*   **Layout**: Grid-based for feature cards. 3 columns on desktop, 2 on tablet, 1 on mobile.
*   **Section Title**: `H2` (`36px`, `font-weight: 700`, `color: #FFFFFF`), centered.
    *   *Example*: "Unlock Unprecedented Trading Insights"
*   **Section Description**: `Body Large` (`18px`, `font-weight: 400`, `color: #A0A0A0`), centered, max-width `768px`.
    *   *Example*: "Our powerful tools provide the edge you need to analyze, learn, and improve your trading strategy."
*   **Feature Card**:
    *   **Container**: `background-color: #1A1A1E`, `border-radius: 8px`, `padding: 32px`, `box-shadow: Shadow-md`.
    *   **Icon**: `48px x 48px`, `color: #00C4B4` (or other accent colors), SVG.
    *   **Title**: `H4` (`22px`, `font-weight: 600`, `color: #FFFFFF`), `margin-top: 16px`.
    *   **Description**: `Body Medium` (`16px`, `font-weight: 400`, `color: #E0E0E0`), `margin-top: 8px`.
    *   *Examples*:
        *   **Card 1**: Icon (Analytics), Title: "Advanced Analytics", Description: "Dive deep into your performance with custom metrics and interactive charts."
        *   **Card 2**: Icon (Backtesting), Title: "Robust Backtesting", Description: "Test strategies against historical data without risking a single dollar."
        *   **Card 3**: Icon (Tracking), Title: "Real-time Performance", Description: "Track every trade, every decision, and see your progress instantly."

### 6.3. Pricing Section

*   **Layout**: Centered content, pricing cards in a row (desktop), stacked (mobile/tablet).
*   **Section Title**: `H2` (`36px`, `font-weight: 700`, `color: #FFFFFF`), centered.
    *   *Example*: "Simple Pricing, Powerful Features"
*   **Section Description**: `Body Large` (`18px`, `font-weight: 400`, `color: #A0A0A0`), centered, max-width `768px`.
    *   *Example*: "Choose the plan that fits your trading style and start optimizing your results today."
*   **Pricing Toggle (Monthly/Annually)**:
    *   **Container**: `background-color: #1A1A1E`, `border-radius: 9999px`, `padding: 4px`, `display: inline-flex`.
    *   **Button (Active)**: `background-color: #2A64F6`, `color: #FFFFFF`, `padding: 8px 24px`, `border-radius: 9999px`, `font-weight: 600`.
    *   **Button (Inactive)**: `background-color: transparent`, `color: #E0E0E0`, `padding: 8px 24px`, `border-radius: 9999px`, `font-weight: 500`.
*   **Pricing Card**:
    *   **Container**: `background-color: #1A1A1E`, `border-radius: 8px`, `padding: 40px`, `box-shadow: Shadow-md`. Highlighted card might have `border: 2px solid #2A64F6`.
    *   **Plan Name**: `H3` (`28px`, `font-weight: 600`, `color: #FFFFFF`).
    *   **Price**: `H1` (`48px`, `font-weight: 800`, `color: #FFFFFF`). Subtext for `/month` or `/year` in `Body Small`, `color: #A0A0A0`.
        *   *Example*: `$49` (H1) `/month` (Body Small)
    *   **Features List**: `Body Medium` (`16px`, `color: #E0E0E0`). Each item prefixed with a checkmark icon (`color: #00E676`). `margin-top: 24px`.
    *   **Call to Action (CTA)**:
        *   **Primary Button**: `background-color: #2A64F6`, `color: #FFFFFF`, `padding: 14px 28px`, `border-radius: 8px`, `font-weight: 600`, `font-size: 16px`.
        *   **Secondary Button (for lower tiers)**: `background-color: transparent`, `border: 1px solid #6C757D`, `color: #E0E0E0`, `padding: 14px 28px`, `border-radius: 8px`, `font-weight: 600`, `font-size: 16px`.

### 6.4. Footer Section

*   **Layout**: Full-width, multi-column on desktop, stacked on mobile.
*   **Background**: `#0A0A0C` (or slightly darker than main background if desired).
*   **Content**:
    *   **Logo**: `height: 40px`, SVG.
    *   **Navigation Links**: Grouped by category (e.g., Product, Company, Resources).
        *   **Category Title**: `H4` (`22px`, `font-weight: 600`, `color: #FFFFFF`).
        *   **Link Item**: `Body Medium` (`16px`, `font-weight: 400`, `color: #A0A0A0`). Hover state: `color: #2A64F6`, `text-decoration: underline`.
    *   **Social Media Links**: Icons (`24px x 24px`, `color: #A0A0A0`). Hover state: `color: #2A64F6`.
    *   **Copyright**: `Body Small` (`14px`, `font-weight: 300`, `color: #A0A0A0`).
        *   *Example*: `© 2023 Premium Trading Journal. All rights reserved.`

---

## 7. Responsive Breakpoints

Standard breakpoints for adapting the layout across various devices.

*   **Mobile**: `max-width: 767px`
    *   Typically single-column layouts, larger text for readability, touch-friendly elements.
*   **Tablet**: `min-width: 768px` and `max-width: 1023px`
    *   Two-column layouts, adjusted spacing, slightly smaller text than desktop.
*   **Desktop**: `min-width: 1024px` and `max-width: 1439px`
    *   Standard multi-column layouts, full feature set.
*   **Large Desktop**: `min-width: 1440px`
    *   Wider layouts, potentially more content density, optimized for large screens.

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Ease-in-out**: Most common easing function for smooth starts and ends.
    *   `transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);`
*   **Ease-out**: For elements that appear quickly and settle.
    *   `transition-timing-function: cubic-bezier(0, 0, 0.2, 1);`
*   **Duration**:
    *   **Short**: `150ms` - For hover states, small color changes, quick feedback.
    *   **Medium**: `250ms` - For component transitions, modal openings/closings, larger state changes.
    *   **Long**: `350ms` - For complex animations or full-page transitions (rare).
*   **Properties**: Animate only necessary properties (e.g., `opacity`, `transform`, `background-color`, `box-shadow`) to ensure performance.
*   **Interactions**:
    *   **Hover**: Subtle `background-color` change, slight `box-shadow` increase, or `transform: translateY(-2px)`.
    *   **Click/Tap**: Quick `scale(0.98)` or `opacity` change for immediate feedback.
    *   **Loading States**: Smooth progress bars or skeleton loaders.
*   **Accessibility**: Ensure animations can be disabled via user preferences (e.g., `prefers-reduced-motion`).

---
```