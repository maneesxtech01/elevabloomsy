# Development Rules & Guidelines - Elevabloomsy

## Code Standard & Formatting Rules

### 1. Liquid Conventions
- Use standard Liquid filters (`image_url`, `t`, `money_with_currency`, `escape`).
- Always assign descriptive local variables at top of snippets (`{%- assign product_form_id = 'product-form-' | append: section.id -%}`).
- Indent Liquid control structures (`{% if %}`, `{% for %}`) cleanly with 2 spaces.
- Use dash tags (`{%- ... -%}`) to reduce unnecessary HTML whitespace.

### 2. Styling (CSS/SCSS)
- Keep design tokens centralized using CSS custom properties (`var(--color-primary)`, `var(--font-heading)`).
- Avoid inline styles; utilize component-specific CSS files inside `/assets/`.
- Ensure responsive layouts use standard flexbox/grid containers with media query breakpoints.

### 3. JavaScript Guidelines
- Write modular ES6+ JavaScript.
- Avoid heavy external dependencies where native web APIs suffice (Custom Elements / Web Components).
- Handle AJAX API promises cleanly with proper try/catch and visual loading states on buttons/drawers.

### 4. Git & Commit Guidelines
- Commit message format: `feat: ...`, `fix: ...`, `docs: ...`, `style: ...`, `refactor: ...`.
- Keep commits atomic and focused on single feature scopes.
- Do not commit generated build artifacts or temporary local environment files.

### 5. Documentation Guidelines
- Maintain all repository technical documentation strictly within `/docs/`.
- File names must strictly adhere to `.md` format (e.g. `PRD.md`, `Architecture.md`, `Rules.md`, `Phases.md`, `Design.md`).
- Do not create `.txt` or `.docx` formats.
