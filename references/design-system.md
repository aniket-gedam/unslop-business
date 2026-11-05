# Premium business website design system

Define a small, coherent system before implementing page sections.

## 1. Color roles

Do not choose colors because they are fashionable. Derive them from the business identity, supplied assets, audience, and positioning.

Define semantic tokens:
- `--color-page`
- `--color-surface`
- `--color-surface-muted`
- `--color-text`
- `--color-text-muted`
- `--color-border`
- `--color-brand`
- `--color-brand-contrast`
- `--color-accent`
- `--color-success`, `--color-warning`, `--color-danger`

Check contrast for text, buttons, and focus indicators. Use a restrained palette with a clear hierarchy.

## 2. Typography

Use a deliberate type system:
- Display: distinctive brand voice, used sparingly.
- Heading: clear hierarchy and consistent rhythm.
- Body: readable at real-world sizes and line lengths.
- UI: compact but legible labels, controls, navigation, and metadata.

Avoid too many font families. If using a remote font, ensure it is licensed/available and provide robust fallbacks. Use fluid sizing where useful, but do not let headings become oversized on small screens.

## 3. Layout

Define:
- Maximum content width.
- Desktop grid and column behavior.
- Mobile gutters.
- Section spacing scale.
- Header height and sticky behavior.
- Image ratios and crop rules.

Use alignment and whitespace intentionally. Avoid placing every section inside a rounded container.

## 4. Components

Build a small set of reusable patterns only where they help:
- Header and navigation.
- Buttons and links.
- Editorial section.
- Product/service item.
- Location/contact block.
- Testimonial or proof block (only with real supplied evidence).
- Form fields and feedback.
- Footer.

Components should support the content's natural shape rather than force all content into identical cards.

## 5. Motion

Motion should explain hierarchy or provide feedback:
- Use short, restrained transitions for hover/focus.
- Avoid animating every element on scroll.
- Avoid parallax unless it genuinely improves the experience.
- Respect `prefers-reduced-motion`.
- Never make essential information depend on animation.

## 6. Responsive behavior

Design mobile as a first-class layout:
- Reconsider navigation, not just shrink it.
- Preserve image focal points.
- Avoid horizontal overflow.
- Keep tap targets comfortable.
- Ensure CTAs remain visible and usable.
- Check long headings, product names, prices, and location details.
