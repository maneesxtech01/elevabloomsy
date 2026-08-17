# Project Memory - Elevabloomsy

## System State & Key Decisions

- **Architecture**: Shopify Online Store 2.0 theme written in Liquid, Vanilla CSS, and lightweight Web Components.
- **Brand Palette**:
  - Primary Accent (Plum): `#6B2C5F`
  - Secondary Highlight (Gold): `#F0B429`
  - Background (Cream): `#FDF8F0`
  - Body & Heading (Dark text): `#121212`
- **Header Transformation**:
  - Replaced legacy header structure with an **Uncommon Goods inspired header design**.
  - Components: Top logo, capsule search bar with cyan spark ✨ + magnifying glass 🔍 icon, dynamic cycling placeholder text (`search | geeky husband gifts, budget is $100`), **live instant predictive search dropdown** (`/search/suggest.json` fetching on 1+ keyup), action bar (`sign in`, `favorites`, `cart`), and streamlined bottom navigation bar.
  - Removed `gift finder` action item per user request.
  - Linked `cart` action item directly to theme slide-out minicart sidebar drawer.
  - Strict performance optimization constraint: lightweight pure Vanilla CSS & JS without heavy third-party libraries.
