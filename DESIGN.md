# Forest Architect Design System

### 1. Overview & Creative North Star
**Creative North Star: The Modern Conservator**
Forest Architect is a high-end editorial design system that bridges the gap between rugged construction and refined architectural precision. It rejects the "standard digital interface" in favor of a layout that feels curated, like a prestige architectural monograph. The system uses deep botanical greens, sun-bleached neutrals, and sharp, intentional typography to create an atmosphere of heritage and stability.

The design breaks the grid through "Structural Asymmetry"—overlapping image cards, large-scale display type that bleeds across sections, and the use of "Polaroid" elements to introduce a human, tactile layer into a technical environment.

### 2. Colors
The palette is rooted in a deep "Forest Green" primary, supported by an "Estate Cream" surface.

*   **Primary Roles:** The primary green (`#133B29`) represents the foundation—used for high-impact sections and core branding. The accent gold (`#E2D43E`) is used sparingly for icons and highlights to signify "architectural highlights."
*   **The "No-Line" Rule:** Visual sectioning must never use 1px solid borders. Instead, use background shifts from `surface` (`#fbf9f8`) to `surface_container_low` (`#f6f3f2`). To separate content, leverage the "Architectural Grid"—a subtle radial dot pattern that defines space without adding visual clutter.
*   **Surface Hierarchy & Nesting:** Use `surface_container_lowest` (Pure White) for "floating" editorial cards (like the Polaroid components) against a `surface` background to create natural separation.
*   **The "Glass & Gradient" Rule:** Navigation and overlay elements should utilize `backdrop-blur-md` with 80% opacity color fills to maintain a sense of environmental depth.

### 3. Typography
The system uses a high-contrast pairing of **Manrope** for structural authority and **Inter** for functional clarity.

*   **Display & Headlines (Manrope):** Large-scale headers use `extrabold` weights with `tracking-tighter` to mimic architectural signage. Reference the 8xl (6rem) and 6xl (3.75rem) scales for hero and section starts.
*   **Body (Inter):** Set in `light` (300) or `regular` (400) weights with `leading-relaxed` (1.625) to ensure maximum legibility against rich backgrounds.
*   **Labels (Inter/Manrope):** Functional labels utilize `uppercase` styling with `tracking-widest` (0.1em to 0.2em) and small sizes (10px to 12px) to create a technical, "blueprint" feel.
*   **Signature Accent (Caveat):** A handwritten cursive is reserved exclusively for photo captions to provide a "Founder's Note" aesthetic.

### 4. Elevation & Depth
Depth is achieved through physical metaphors rather than standard digital shadows.

*   **The Layering Principle:** Components are stacked using "Z-index storytelling." For example, a quote box may overlap an image container to create a three-dimensional composition.
*   **Ambient Shadows:** Based on the ground truth data, utilize extra-diffused shadows for interactive elements:
    *   *Standard Card:* `0 4px 20px rgba(0, 0, 0, 0.08)`
    *   *Elevated/Hover:* `0 20px 40px rgba(0, 0, 0, 0.12)`
*   **The "Ghost Border" Fallback:** For input fields and containers on dark backgrounds, use a `white/30` or `white/10` border to provide a subtle "etched" look without heavy lines.

### 5. Components
*   **Buttons:** Rectangular with `rounded-lg` (0.25rem). Primary buttons use a vibrant tertiary green (`#50ca90`) that transitions to the gold accent on hover, creating a high-energy interaction.
*   **Polaroid Cards:** A signature component. A white container with generous bottom padding for `Caveat` typography, utilizing a grayscale-to-color filter transition on hover.
*   **Input Fields:** Ghost-style inputs with semi-transparent backgrounds (`white/10`) and subtle white borders. Focus states should exclusively use the accent gold.
*   **Iconography:** Use Material Symbols in "Outlined" style with a weight of 400. Icons should frequently be used as decorative oversized elements in high-contrast colors.

### 6. Do's and Don'ts
*   **Do:** Use "Structural Overlap" (elements partially covering others) to create depth.
*   **Do:** Use the 884px hero height to create a cinematic entry point.
*   **Don't:** Use rounded corners exceeding 12px unless it is a specialized "pill" label. The system favors architectural rigidity.
*   **Don't:** Use black for text. Use `on_surface` (`#1b1c1c`) or `on_surface_variant` (`#414843`) to maintain the "bleached" editorial tone.
*   **Do:** Apply `grayscale` and `contrast-125` filters to hero imagery to ensure text legibility and a consistent brand mood.