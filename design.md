# Design System Strategy: Ethereal Terminal

## 1. Overview & Creative North Star
**Creative North Star: The Sovereign HUD (Heads-Up Display)**

This design system is not a standard web dashboard; it is a high-performance instrument. For the professional daytrader, clarity is profit and latency is loss. We move beyond "template" aesthetics by adopting a **Sovereign HUD** philosophyâ€”a layout that feels like a singular, integrated piece of glass rather than a collection of boxes.

We break the grid through **Intentional Asymmetry**. Key performance indicators (KPIs) should not just sit in rows; they should "float" with varying tonal depths. By using overlapping glass surfaces and a high-contrast typography scale, we create a technical, editorial experience that feels both authoritative and ethereal. The interface should feel like a dark room where only the most vital data glows.

---

## 2. Colors & Atmospheric Depth
The palette is rooted in a "Deep Space" black, utilizing the Electric Blue and Magenta accents not as mere decorations, but as functional status indicators (Bullish vs. Bearish / Profit vs. Loss).

### The "No-Line" Rule
**Borders are a design failure in this system.** Do not use 1px solid strokes to separate sections. Structure must be defined through:
- **Tonal Shifts:** Placing a `surface-container-high` card against a `surface-dim` background.
- **Negative Space:** Utilizing the Spacing Scale (specifically `spacing-8` and `spacing-10`) to create breathing room that defines boundaries.
- **Shadow Depth:** Using ambient, tinted glows to lift a container rather than outlining it.

### Surface Hierarchy & Nesting
Treat the UI as a series of stacked, frosted obsidian sheets.
*   **Base Layer:** `surface` (#0b0e14) â€” The infinite void.
*   **Section Layer:** `surface-container-low` (#10131a) â€” Large structural areas (e.g., Sidebars).
*   **Component Layer:** `surface-container-high` (#1c2028) â€” Individual trade cards or data modules.
*   **Active/Interaction Layer:** `surface-bright` (#282c36) â€” Focused elements or hovered states.

### The Glass & Gradient Rule
For high-level metrics (Win Rate, Profit Factor), use **Glassmorphism**. Combine `surface-container-highest` at 40% opacity with a `backdrop-blur` of 20px. 
*   **Signature Glow:** Apply a subtle linear gradient from `primary` (#72dcff) to `primary-container` (#00d2ff) at 10% opacity as a background fill for hero metrics to give them a "powered-on" technical soul.

---

## 3. Typography: Technical Authority
We use **Manrope** exclusively. Its geometric construction provides the "Modern Technical" feel required for rapid data ingestion.

*   **Display (The Pulse):** `display-lg` (3.5rem) should be used for the Daily P&L. It must be bold and commanding.
*   **Headlines (The Context):** `headline-sm` (1.5rem) for section titles like "Trade Distribution." Use tighter letter-spacing (-0.02em) to enhance the premium, editorial feel.
*   **Data Labels (The Precision):** `label-md` (0.75rem) using `on-surface-variant` (#a9abb3) in All-Caps for secondary metadata. This creates a "terminal" aesthetic.
*   **The Hierarchy Rule:** Never pair two font sizes that are adjacent in the scale (e.g., don't put `title-md` next to `title-sm`). Jump levels to create a high-contrast, professional tension.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are forbidden. We use **Ambient Radiance**.

*   **Layering Principle:** Achieve depth by "nesting" tokens. A `surface-container-lowest` (#000000) data table sitting inside a `surface-container-low` (#10131a) dashboard creates a "recessed" look, ideal for secondary data.
*   **Ambient Shadows:** For floating modals, use a large blur (40px+) with a 6% opacity shadow tinted with `primary` (#72dcff). It should feel like the component is emitting light onto the surface below, not casting a shadow.
*   **Ghost Borders:** If a separator is required for accessibility, use `outline-variant` (#45484f) at **15% opacity**. It should be felt, not seen.

---

## 5. Components & Interface Elements

### Buttons (The Interaction Triggers)
*   **Primary:** Solid `primary_container` (#00d2ff). Use `rounded-sm` (0.125rem) for a sharp, precision-tool look. No rounded "pill" buttons unless they are secondary chips.
*   **Secondary:** Ghost style. `outline` color with a `primary` glow on hover.

### Data Cards (The Core Module)
*   **Forbid Dividers:** Do not use lines to separate "Entry Price" from "Exit Price." Use a 2-column layout with `spacing-4` (0.9rem) gaps. 
*   **Dynamic Glow:** Cards containing "Winning Trades" should have a subtle 2px left-border glow using `primary` (#72dcff). "Losing Trades" use `secondary` (#ff51fa).

### Trading Inputs
*   **Input Fields:** `surface-container-highest` background with a `none` border. On focus, the background transitions to `surface-bright` and a `primary` 1px bottom-bar appears (not a full box).
*   **Selection Chips:** Use `rounded-full` (9999px) to contrast with the sharp-edged data cards. This makes interactive filters feel distinct from static data.

### Signature Component: The "Performance Ribbon"
A horizontal, semi-transparent `glassmorphism` bar that sits at the top of the terminal, housing real-time equity curves. Use a `primary` to `secondary` gradient for the line graph to represent the "Ethereal" brand identity.

---

## 6. Do's and Don'ts

### Do
*   **Do** use `primary` (#72dcff) for bullish/positive data and `secondary` (#ff51fa) for bearish/negative data. This is the core "Ethereal Terminal" visual language.
*   **Do** lean into asymmetry. A large metric on the left balanced by three small metrics on the right feels more "professional" than a 4-column grid.
*   **Do** use `on-surface-variant` (#a9abb3) for labels to ensure the `on-surface` (#ecedf6) data values pop with maximum contrast.

### Don't
*   **Don't** use a standard 8px grid. Use the custom spacing scale (e.g., `spacing-3.5` at 0.75rem) to find the "tension" between data-density and whitespace.
*   **Don't** ever use #000000 for text. It kills the "glow" effect. Use `on-surface` for all primary reading.
*   **Don't** use 100% opaque borders. They create visual "noise" that distracts a trader during high-volatility sessions.