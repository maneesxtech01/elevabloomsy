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
  - Announcement Bar: Single looping headline `✨ Handmade Gifts & Premium Smart Watches | COD Available Across Pakistan ✨` in `#6B2C5F` background.
  - Desktop View: Logo left, capsule search bar center (cyan spark ✨ + magnifier 🔍, live predictive search with `z-index: 999999`), action links right (`sign in`, `favorites`, `cart`). **Strictly no hamburger menu on desktop**.
  - Mobile View: Theme default mobile layout with `SHOP ☰` toggle on left (triggering native side drawer menu & categories), logo in center, action icons & capsule search.
  - Linked `cart` action item directly to theme slide-out minicart sidebar drawer.
  - Strict performance optimization constraint: lightweight pure Vanilla CSS & JS without heavy third-party libraries.
