This `design.md` file outlines the core design system for the "Premium Trading Journal" SaaS project. It provides specific guidelines for an AI coder to reference during implementation, ensuring consistency and adherence to the brand's aesthetic.

---

# Design System: Premium Trading Journal

## Project Overview
A premium trading journal for daytraders, offering advanced analytics such as P&L tracking, win-rate breakdown, backtesting capabilities, and equity curve visualization.

## Style & Tone
**Type:** SaaS
**Style:** Dark, professional, sophisticated, data-driven, clean, and modern.
**Tone:** Trustworthy, empowering, analytical, high-performance.

---

## 1. Color Palette

The color palette is designed to be dark and sleek, with vibrant accents for data visualization and interactive elements.

*   **Background:**
    *   `--color-background-primary`: `#0A0A0C` (Deepest dark grey, almost black)
    *   `--color-background-secondary`: `#1A1A1E` (Slightly lighter dark grey for cards/surfaces)
    *   `--color-background-tertiary`: `#2D2D32` (Dark grey for subtle differentiation)
*   **Text:**
    *   `--color-text-primary`: `#E2E8F0` (Light grey for main content)
    *   `--color-text-secondary`: `#A0AEC0` (Medium grey for secondary information, captions)
    *   `--color-text-disabled`: `#6B7280` (Darker grey for disabled states)
*   **Primary Accent:**
    *   `--color-accent-primary`: `#6366F1` (Indigo - for main CTAs, active states, key highlights)
    *   `--color-accent-primary-hover`: `#4F46E5` (Darker Indigo for hover states)
*   **Secondary Accent:**
    *   `--color-accent-secondary`: `#8B5CF6` (Violet - for secondary CTAs, subtle interactive elements)
*   **Border & Divider:**
    *   `--color-border`: `#374151` (Dark grey for borders and separators)
*   **Status & Data Visualization:**
    *   `--color-success`: `#10B981` (Emerald Green - for profit, positive metrics)
    *   `--color-error`: `#EF4444` (Red - for loss, negative metrics, error messages)
    *   `--color-warning`: `#F59E0B` (Amber - for warnings, neutral alerts)
    *   `--color-info`: `#3B82F6` (Blue - for informational messages)

---

## 2. Typography

Using a single, highly readable sans-serif font for consistency and modern appeal.

*   **Font Family:**
    *   `--font-family-primary`: `'Inter', sans-serif`
*   **Headings (Font Weight: 700 - Bold):**
    *   `--font-size-h1`: `48px` (`line-height: 1.2`)
    *   `--font-size-h2`: `36px` (`line-height: 1.25`)
    *   `--font-size-h3`: `30px` (`line-height: 1.3`)
    *   `--font-size-h4`: `24px` (`line-height: 1.35`)
    *   `--font-size-h5`: `20px` (`line-height: 1.4`)
    *   `--font-size-h6`: `18px` (`line-height: 1.45`)
*   **Body Text (Font Weight: 400 - Regular):**
    *   `--font-size-body-lg`: `18px` (`line-height: 1.6`)
    *   `--font-size-body-md`: `16px` (`line-height: 1.6`)
    *   `--font-size-body-sm`: `14px` (`line-height: 1.6`)
*   **Caption & Small Text (Font Weight: 400 - Regular):**
    *   `--font-size-caption`: `12px` (`line-height: 1.5`)
*   **Button Text (Font Weight: 600 - Semi-bold):**
    *   `--font-size-button-lg`: `18px`
    *   `--font-size-button-md`: `16px`
    *   `--font-size-button-sm`: `14px`

---

## 3. Spacing Scale

A consistent 4px-based spacing scale for all elements.

*   `--spacing-xs`: `4px`
*   `--spacing-sm`: `8px`
*   `--spacing-md`: `16px`
*   `--spacing-lg`: `24px`
*   `--spacing-xl`: `32px`
*   `--spacing-xxl`: `48px`
*   `--spacing-xxxl`: `64px`
*   `--spacing-xxxxl`: `96px`

---

## 4. Border Radius

Subtle rounded corners for a modern, friendly, yet professional feel.

*   `--border-radius-sm`: `4px`
*   `--border-radius-md`: `8px`
*   `--border-radius-lg`: `12px`
*   `--border-radius-full`: `9999px` (for pills, avatars)

---

## 5. Shadow Styles

Subtle, dark shadows to provide depth and hierarchy without being distracting.

*   `--shadow-sm`: `0 1px 2px 0 rgba(0, 0, 0, 0.2), 0 1px 1px 0 rgba(0, 0, 0, 0.1)`
*   `--shadow-md`: `0 4px 6px -1px rgba(0, 0, 0, 0.2), 0 2px 4px -1px rgba(0, 0, 0, 0.1)`
*   `--shadow-lg`: `0 10px 15px -3px rgba(0, 0, 0, 0.3), 0 4px 6px -2px rgba(0, 0, 0, 0.2)`
*   `--shadow-inset`: `inset 0 2px 4px 0 rgba(0, 0, 0, 0.06)`

---

## 6. Component Specifications by Section

### Global Components

*   **Buttons:**
    *   **Primary:** `background: var(--color-accent-primary); color: var(--color-text-primary); border-radius: var(--border-radius-md); padding: var(--spacing-md) var(--spacing-lg); font-size: var(--font-size-button-md); font-weight: 600; transition: all 0.2s ease-in-out;`
        *   `Hover:` `background: var(--color-accent-primary-hover);`
    *   **Secondary:** `background: transparent; color: var(--color-accent-primary); border: 1px solid var(--color-accent-primary); border-radius: var(--border-radius-md); padding: var(--spacing-md) var(--spacing-lg); font-size: var(--font-size-button-md); font-weight: 600; transition: all 0.2s ease-in-out;`
        *   `Hover:` `background: rgba(99, 102, 241, 0.1);`
    *   **Tertiary (Text-only):** `background: transparent; color: var(--color-text-secondary); font-size: var(--font-size-button-sm); font-weight: 600; transition: all 0.2s ease-in-out;`
        *   `Hover:` `color: var(--color-text-primary);`
*   **Input Fields:** `background: var(--color-background-secondary); border: 1px solid var(--color-border); color: var(--color-text-primary); border-radius: var(--border-radius-sm); padding: var(--spacing-sm) var(--spacing-md); font-size: var(--font-size-body-md);`
    *   `Focus:` `border-color: var(--color-accent-primary); box-shadow: 0 0 0 2px rgba(99, 102, 241, 0.2);`
*   **Cards:** `background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: var(--spacing-xl); box-shadow: var(--shadow-md);`

### Section: Hero

*   **Layout:** Full-width section. Left-aligned text content (Headline, Subheadline, CTAs), right-aligned visual (product screenshot/mockup).
*   **Headline:** `h1` (`--font-size-h1`), `color: var(--color-text-primary);`
*   **Subheadline:** `body-lg` (`--font-size-body-lg`), `color: var(--color-text-secondary);`
*   **Call-to-Action (CTA) Buttons:** Two buttons, Primary (e.g., "Start Free Trial") and Secondary (e.g., "Learn More").
*   **Visual:** High-fidelity mockup of the trading journal UI on a dark device frame. `max-width: 600px; height: auto;`

### Section: Features

*   **Layout:** Grid-based layout (e.g., 3 columns on desktop, 2 on tablet, 1 on mobile).
*   **Feature Card:**
    *   `background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: var(--spacing-xl); text-align: center;`
    *   **Icon:** `color: var(--color-accent-primary); font-size: 48px; margin-bottom: var(--spacing-md);`
    *   **Title:** `h4` (`--font-size-h4`), `color: var(--color-text-primary); margin-bottom: var(--spacing-sm);`
    *   **Description:** `body-md` (`--font-size-body-md`), `color: var(--color-text-secondary);`

### Section: Pricing

*   **Layout:** Flexbox or Grid for pricing cards (e.g., 3 columns on desktop).
*   **Pricing Card:**
    *   `background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: var(--spacing-xl); text-align: center; border: 1px solid var(--color-border);`
    *   **"Most Popular" Highlight:** `border-color: var(--color-accent-primary); box-shadow: var(--shadow-lg);`
    *   **Plan Name:** `h3` (`--font-size-h3`), `color: var(--color-text-primary); margin-bottom: var(--spacing-sm);`
    *   **Price:** `h1` (`--font-size-h1`), `color: var(--color-text-primary); font-weight: 700;` (e.g., "$49")
        *   `Suffix (per month/year):` `body-md` (`--font-size-body-md`), `color: var(--color-text-secondary);`
    *   **Features List:** Unordered list, `body-md` (`--font-size-body-md`), `color: var(--color-text-secondary);`
        *   Each item with a checkmark icon (`color: var(--color-success);`).
    *   **CTA Button:** Primary button, `margin-top: var(--spacing-xl);`
*   **Monthly/Annual Toggle:** `background: var(--color-background-tertiary); border-radius: var(--border-radius-full); padding: var(--spacing-xs); display: inline-flex;`
    *   `Active state:` `background: var(--color-accent-primary); color: var(--color-text-primary);`
    *   `Inactive state:` `background: transparent; color: var(--color-text-secondary);`

### Section: Testimonials

*   **Layout:** Carousel or grid of testimonial cards.
*   **Testimonial Card:**
    *   `background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: var(--spacing-xl);`
    *   **Quote:** `body-lg` (`--font-size-body-lg`), `color: var(--color-text-primary); font-style: italic; margin-bottom: var(--spacing-lg);`
    *   **Author Info:**
        *   **Avatar:** `width: 56px; height: 56px; border-radius: var(--border-radius-full); margin-right: var(--spacing-md);`
        *   **Name:** `h6` (`--font-size-h6`), `color: var(--color-text-primary);`
        *   **Title/Company:** `body-sm` (`--font-size-body-sm`), `color: var(--color-text-secondary);`

### Section: FAQ

*   **Layout:** Accordion style.
*   **FAQ Item:**
    *   **Question (Header):** `h5` (`--font-size-h5`), `color: var(--color-text-primary); padding: var(--spacing-md) 0; cursor: pointer; display: flex; justify-content: space-between; align-items: center; border-bottom: 1px solid var(--color-border);`
        *   `Icon (chevron):` `color: var(--color-text-secondary); transition: transform 0.2s ease-in-out;`
        *   `Active state:` `transform: rotate(180deg);`
    *   **Answer (Content):** `body-md` (`--font-size-body-md`), `color: var(--color-text-secondary); padding: var(--spacing-md) 0 var(--spacing-xl) 0; overflow: hidden; transition: max-height 0.3s ease-in-out;` (Initially `max-height: 0;`)

### Section: Contact

*   **Layout:** Two columns (form on left, contact info/social on right) on desktop, stacked on mobile/tablet.
*   **Contact Form:**
    *   `background: var(--color-background-secondary); border-radius: var(--border-radius-lg); padding: var(--spacing-xl);`
    *   **Labels:** `body-sm` (`--font-size-body-sm`), `color: var(--color-text-secondary); margin-bottom: var(--spacing-xs);`
    *   **Input Fields:** Standard input field styles.
    *   **Textarea:** Same as input, but `min-height: 120px; resize: vertical;`
    *   **Submit Button:** Primary button.
*   **Contact Info:**
    *   `h4` (`--font-size-h4`), `color: var(--color-text-primary); margin-bottom: var(--spacing-md);`
    *   `body-md` (`--font-size-body-md`), `color: var(--color-text-secondary);`
    *   **Social Links:** Icons (`font-size: 24px; color: var(--color-text-secondary);`) with `margin-right: var(--spacing-md);`
        *   `Hover:` `color: var(--color-accent-primary);`

### Section: Footer

*   **Layout:** Multi-column on desktop (Logo/Copyright, Nav links, Social links), stacked on mobile.
*   **Background:** `var(--color-background-primary);`
*   **Text:** `body-sm` (`--font-size-body-sm`), `color: var(--color-text-secondary);`
*   **Logo:** SVG or image, `height: 32px;`
*   **Navigation Links:** `color: var(--color-text-secondary); text-decoration: none;`
    *   `Hover:` `color: var(--color-text-primary);`
*   **Social Media Icons:** Same as Contact section.

---

## 7. Responsive Breakpoints

Standard breakpoints for adapting layout across devices.

*   **Mobile:** `0px` to `767px`
*   **Tablet:** `768px` to `1023px`
*   **Desktop:** `1024px` to `1439px`
*   **Large Desktop:** `1440px` and above

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance user experience without being distracting or slowing down performance.

*   **Timing Function:** `ease-in-out` for most transitions.
*   **Duration:** `200ms` to `300ms` for most interactive elements (hovers, clicks, toggles).
*   **Types of Animations:**
    *   **Hover Effects:** Subtle background changes, border highlights, or slight scaling on interactive elements (buttons, cards, links).
    *   **Focus States:** Clear visual indication for keyboard navigation.
    *   **Content Reveals:** Smooth transitions for accordions, modals, or loading states.
    *   **Micro-interactions:** Small, delightful animations on success/error messages, form submissions.
*   **Performance:** Prioritize CSS transforms and opacity changes for smooth animations. Avoid animating properties that cause layout reflows where possible.
*   **Accessibility:** Ensure animations can be disabled or reduced for users with motion sensitivities (e.g., via `prefers-reduced-motion` media query).

---