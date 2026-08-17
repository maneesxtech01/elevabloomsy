# Design System Document - Elevabloomsy

## Visual Aesthetics & Palette

Elevabloomsy features a refined, high-end floral & lifestyle design aesthetic characterized by warm neutral tones, organic botanical accents, smooth micro-interactions, and visual harmony.

### Color Palette

| Name | Hex / Variable | Usage |
| :--- | :--- | :--- |
| **Plum** | `#6B2C5F` / `--color-primary` | Primary brand accent, primary CTA buttons |
| **Gold** | `#F0B429` / `--color-secondary` | Highlights, ratings, special badges |
| **Cream** | `#FDF8F0` / `--color-bg-primary` | Main page background, section fills |
| **Dark Text** | `#121212` / `--color-text` | Primary headings, body copy, dark elements |
| **Muted Border** | `#E7E5E4` / `--color-border` | Subtle divider lines, card borders |

---

## Typography

- **Headings**: Serif family (Playfair Display / Cormorant Garamond) for luxury floral branding.
- **Body & UI**: Sans-Serif family (Inter / Jost) for crisp legibility across sizes.

---

## UI Components & Micro-Interactions

### 1. Product Cards & Grid
- Smooth image zoom on hover (`transform: scale(1.04); transition: transform 0.4s ease`).
- Quick view & Add to Cart action buttons overlaying card footer on hover.

### 2. Slide-out Drawers
- Soft backdrop blur filter (`backdrop-filter: blur(8px);`).
- Smooth cubic-bezier slide-in animation for cart and mobile navigation menu.

### 3. Buttons & Controls
- Pill-shaped CTAs with subtle glow or shadow shift on hover.
- Accessible focus states for key accessibility compliance.
