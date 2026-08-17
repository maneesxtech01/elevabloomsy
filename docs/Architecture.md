# Architecture Document - Elevabloomsy

## Directory Structure & System Layout

Elevabloomsy is structured according to Shopify Online Store 2.0 specifications:

```
elevabloomsy/
├── assets/         # CSS stylesheets, JavaScript modules, fonts, SVGs
├── config/         # settings_schema.json, settings_data.json
├── layout/         # Base layout files (theme.liquid, password.liquid)
├── locales/        # Translation files (en.default.json, etc.)
├── sections/       # Dynamic & static customizable sections
├── snippets/       # Reusable Liquid components & SVG icons
├── templates/      # JSON page templates and customer account layouts
└── docs/           # Project technical documentation
```

---

## Core Components Breakdown

### 1. Layout Engine (`/layout`)
- **`theme.liquid`**: Primary html container defining header script injections, main layout wrapper, global overlays, slide-out minicart snippet, search drawer, and footer rendering.

### 2. Sections Layer (`/sections`)
- Modular sections configurable via the Shopify theme editor:
  - Header & Navigation menus
  - Hero Banners & Slideshows
  - Featured Product Grid & Collections
  - Promotional Marquees & Customer Reviews
  - Footer & Newsletter subscription

### 3. Snippets Library (`/snippets`)
- Atomic reusable elements including `product-item.liquid`, `price.liquid`, `responsive-image.liquid`, `minicart.liquid`, `social-icons.liquid`, and vector icons (`icon-*.liquid`).

### 4. Customizer Configuration (`/config`)
- **`settings_schema.json`**: Defs for colors, typography, layout container widths, social links, and checkout settings usable across sections.

---

## Data Flow & State Management

```
[ Shopify Storefront API / Liquid Context ]
                     │
                     ▼
           [ Theme Liquid Engine ]
                     │
                     ▼
      [ HTML5 / CSS / Vanilla JavaScript ]
                     │
       ┌─────────────┴─────────────┐
       ▼                           ▼
[ Dynamic Swiper / UI ]     [ AJAX Cart & Search API ]
```

- **AJAX Drawer State**: Cart updates perform asynchronous POST/GET requests to `/cart/add.js`, `/cart/change.js`, and update drawer DOM elements without full page reloads.
- **Predictive Search**: Uses `/search/suggest.json` for live auto-complete querying.
