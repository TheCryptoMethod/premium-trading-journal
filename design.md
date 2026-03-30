# Design System Documentation

This document outlines the core design principles and specifications for the premium trading journal SaaS project. It serves as a single source of truth for UI/UX elements, ensuring consistency and efficiency in development.

---

## 1. Project Overview

**Project Name:** Premium Trading Journal
**Type:** SaaS
**Style:** Dark, Modern, Professional
**Description:** A sophisticated trading journal for daytraders, featuring advanced analytics, backtesting, and a sleek dark-themed interface.

---

## 2. Color Palette

A carefully selected dark color scheme with a vibrant accent to highlight key actions and data.

*   **Background:** `#0A0A0F` (Deep Charcoal - Main page background)
*   **Primary (UI Elements):** `#1A1A22` (Dark Grey - Card backgrounds, primary containers)
*   **Secondary (Borders, Subtle Accents):** `#2C2C38` (Medium Dark Grey - Borders, dividers, secondary UI elements)
*   **Accent (Interactive Elements):** `#00C896` (Vibrant Teal - CTAs, highlights, active states, key data points)
*   **Text Primary:** `#E0E0E6` (Off-White - Main body text, headings)
*   **Text Secondary:** `#A0A0A8` (Light Grey - Secondary text, labels, disabled states)
*   **Success:** `#34D399` (Green - Positive feedback, success messages)
*   **Error:** `#EF4444` (Red - Negative feedback, error messages)
*   **Warning:** `#FBBF24` (Amber - Warning messages, alerts)

---

## 3. Typography

Using a single, versatile font family for consistency and readability across all elements.

*   **Font Family:** `Inter`, sans-serif
    *   **Fallback:** `system-ui`, `-apple-system`, `BlinkMacSystemFont`, `"Segoe UI"`, `Roboto`, `"Helvetica Neue"`, `Arial`, `"Noto Sans"`, `sans-serif`, `"Apple Color Emoji"`, `"Segoe UI Emoji"`, `"Segoe UI Symbol"`, `"Noto Color Emoji"`
*   **Font Weights Used:** Regular (400), Medium (500), SemiBold (600), Bold (700)

### Font Sizes (Desktop Base)

*   **H1 (Hero Titles):** `48px` (Bold)
*   **H2 (Section Titles):** `36px` (SemiBold)
*   **H3 (Card Titles, Sub-sections):** `28px` (Medium)
*   **H4 (Minor Headings):** `22px` (Medium)
*   **Body Large:** `18px` (Regular)
*   **Body:** `16px` (Regular - Default text size)
*   **Small:** `14px` (Regular - Captions, meta info)

### Line Heights

*   Headings: `1.2`
*   Body Text: `1.5`

---

## 4. Spacing Scale

A consistent 8px-based spacing scale for all layout and component spacing.

*   **xs:** `8px`
*   **sm:** `16px`
*   **md:** `24px`
*   **lg:** `48px`
*   **xl:** `80px`
*   **xxl:** `120px` (For large section padding)

---

## 5. Border Radius

Subtle rounding for a modern and friendly feel, without being overly soft.

*   **Default:** `8px` (For cards, buttons, input fields)
*   **Small:** `4px` (For smaller elements, badges)
*   **Full:** `9999px` (For pill-shaped elements, avatars)

---

## 6. Shadow Styles

Subtle, dark shadows to provide depth and hierarchy in the dark interface.

*   **Small Shadow (Subtle Lift):**
    *   `box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.2);`
*   **Medium Shadow (Card Elevation):**
    *   `box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.3);`
*   **Large Shadow (Modal, Popover):**
    *   `box-shadow: 0px 8px 24px rgba(0, 0, 0, 0.4);`

---

## 7. Component Specifications

Detailed specifications for key sections of the landing page.

### 7.1. Hero Section

*   **Background:** `Background` color (`#0A0A0F`) with a subtle gradient or pattern for depth.
*   **Container:** Max-width `1280px`, centered, `xl` padding top/bottom.
*   **Heading (H1):**
    *   Font: `Inter`, `48px`, `Bold`.
    *   Color: `Text Primary` (`#E0E0E6`).
    *   Key phrase/word within heading to use `Accent` color (`#00C896`).
*   **Subheading (Body Large):**
    *   Font: `Inter`, `18px`, `Regular`.
    *   Color: `Text Secondary` (`#A0A0A8`).
    *   Spacing: `md` margin-top from H1.
*   **Call to Action (CTA) Button:**
    *   Background: `Accent` color (`#00C896`).
    *   Text Color: `Background` color (`#0A0A0F`).
    *   Padding: `16px` vertical, `32px` horizontal.
    *   Border Radius: `8px`.
    *   Font: `Inter`, `18px`, `SemiBold`.
    *   Hover: Background darkens slightly (`#00A37A`), subtle `Medium Shadow`.
    *   Spacing: `lg` margin-top from subheading.
*   **Supporting Image/Mockup:**
    *   High-quality screenshot or illustration of the app interface, dark-themed.
    *   Positioned to complement text, potentially floating or slightly overlapping.

### 7.2. Features Section

*   **Background:** `Primary (UI Elements)` color (`#1A1A22`).
*   **Section Title (H2):**
    *   Font: `Inter`, `36px`, `SemiBold`.
    *   Color: `Text Primary` (`#E0E0E6`).
    *   Centered.
    *   Spacing: `xl` padding top/bottom for the section.
*   **Feature Grid:**
    *   Layout: Responsive grid (e.g., 3 columns desktop, 2 columns tablet, 1 column mobile).
    *   Gap: `lg` between cards.
*   **Feature Card:**
    *   Background: `Primary (UI Elements)` color (`#1A1A22`).
    *   Border: `1px` solid `Secondary (Borders)` color (`#2C2C38`).
    *   Border Radius: `8px`.
    *   Padding: `lg`.
    *   Shadow: `Medium Shadow`.
    *   **Icon:**
        *   Size: `48px` x `48px`.
        *   Color: `Accent` color (`#00C896`).
        *   Spacing: `md` margin-bottom.
    *   **Title (H3):**
        *   Font: `Inter`, `28px`, `Medium`.
        *   Color: `Text Primary` (`#E0E0E6`).
        *   Spacing: `sm` margin-bottom.
    *   **Description (Body):**
        *   Font: `Inter`, `16px`, `Regular`.
        *   Color: `Text Secondary` (`#A0A0A8`).

### 7.3. Pricing Section

*   **Background:** `Background` color (`#0A0A0F`).
*   **Section Title (H2):**
    *   Font: `Inter`, `36px`, `SemiBold`.
    *   Color: `Text Primary` (`#E0E0E6`).
    *   Centered.
    *   Spacing: `xl` padding top/bottom for the section.
*   **Pricing Grid:**
    *   Layout: Responsive grid (e.g., 3 columns desktop, 1-2 columns tablet/mobile).
    *   Gap: `lg` between cards.
*   **Pricing Card:**
    *   Background: `Primary (UI Elements)` color (`#1A1A22`).
    *   Border: `1px` solid `Secondary (Borders)` color (`#2C2C38`).
    *   Border Radius: `8px`.
    *   Padding: `lg`.
    *   Shadow: `Medium Shadow`.
    *   **Plan Name (H3):**
        *   Font: `Inter`, `28px`, `Medium`.
        *   Color: `Text Primary` (`#E0E0E6`).
        *   Centered.
        *   Spacing: `md` margin-bottom.
    *   **Price:**
        *   Font: `Inter`, `48px`, `Bold`.
        *   Color: `Accent` color (`#00C896`).
        *   Centered.
        *   Suffix (e.g., "/month"): `Text Secondary`, `18px`.
        *   Spacing: `md` margin-bottom.
    *   **Features List:**
        *   Unordered list.
        *   List Item Font: `Inter`, `16px`, `Regular`.
        *   List Item Color: `Text Primary` (`#E0E0E6`).
        *   Icon (checkmark): `Accent` color (`#00C896`).
        *   Spacing: `sm` vertical spacing between items.
        *   Spacing: `lg` margin-bottom for the list.
    *   **CTA Button:**
        *   Style: Same as Hero CTA, but potentially `100%` width within the card.
        *   Text: "Choose Plan" or "Start Free Trial".
    *   **"Most Popular" Badge (Optional):**
        *   Position: Top-right corner of the card.
        *   Background: `Accent` color (`#00C896`).
        *   Text Color: `Background` color (`#0A0A0F`).
        *   Font: `Inter`, `14px`, `SemiBold`.
        *   Padding: `xs` vertical, `sm` horizontal.
        *   Border Radius: `Full`.
        *   Applied to one specific pricing card.

### 7.4. Footer Section

*   **Background:** `Background` color (`#0A0A0F`).
*   **Padding:** `xl` top/bottom.
*   **Layout:** Grid or flexbox for columns (e.g., logo, navigation, legal, social).
*   **Logo:** Project logo (white/light version).
*   **Navigation Links:**
    *   Font: `Inter`, `16px`, `Regular`.
    *   Color: `Text Secondary` (`#A0A0A8`).
    *   Hover: `Accent` color (`#00C896`).
    *   Spacing: `sm` vertical spacing.
*   **Copyright Text:**
    *   Font: `Inter`, `14px`, `Regular`.
    *   Color: `Text Secondary` (`#A0A0A8`).
*   **Social Media Icons:**
    *   Icons: SVG or icon font.
    *   Color: `Text Secondary` (`#A0A0A8`).
    *   Hover: `Accent` color (`#00C896`).
    *   Size: `24px` x `24px`.
    *   Spacing: `sm` horizontal spacing.

---

## 8. Responsive Breakpoints

Standard breakpoints for adapting the layout across devices.

*   **Mobile:** `0px` - `767px`
    *   Layouts typically stack vertically.
    *   Font sizes may be reduced (e.g., H1: `36px`, Body: `15px`).
    *   Padding and margins reduced (e.g., `lg` becomes `md`).
*   **Tablet:** `768px` - `1023px`
    *   Layouts may start to use multiple columns (e.g., 2-column grids).
    *   Font sizes closer to desktop, but potentially slightly smaller.
*   **Desktop:** `1024px` and up
    *   Full desktop layouts.
    *   Max content width `1280px` for main sections.

---

## 9. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Duration:** Short to medium (`150ms` - `300ms`).
*   **Easing:** `ease-in-out` for most transitions.
*   **Types of Animations:**
    *   **Hover Effects:** Buttons, links, cards should have subtle color changes, slight lifts (`Small Shadow`), or scale transformations.
    *   **Focus States:** Clear visual indication for keyboard navigation.
    *   **Transitions:** Smooth transitions for state changes (e.g., menu open/close, tab switching).
    *   **Loading States:** Minimalistic loaders or skeleton screens.
*   **Avoid:** Excessive bouncing, flashing, or overly complex animations. Performance is key.