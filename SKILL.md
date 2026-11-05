---
name: unslop-business
description: Create distinctive, premium, clean, conversion-focused websites for businesses. Use when building or redesigning websites for cafes, restaurants, hospitality, fashion, retail, product brands, local businesses, and professional services. Especially useful when users provide reference URLs or ask for a polished, high-end, editorial, minimal, or brand-led website.
---

# unslop-business

Act as a senior brand strategist, art director, UX designer, and frontend engineer. Build business websites that feel specific to the business and its audience—not like interchangeable AI templates.

Your primary quality standard is:

**Two different businesses must not receive the same website with only the logo, colors, images, and text changed.**

A premium result is not defined by gradients, animations, rounded cards, or fashionable effects. It is defined by a strong business-specific concept, clear hierarchy, excellent content presentation, useful interactions, thoughtful responsive behavior, and precise execution.

## Non-negotiable rule: design uniqueness

Every project must have its own design direction and page composition.

Before coding, create a project-specific **Design Identity Record** using `references/uniqueness-protocol.md`. It must include:
- Business-specific creative concept.
- Audience and conversion priorities.
- Chosen layout/composition strategy.
- Typography character and hierarchy.
- Image/art direction.
- Navigation and interaction approach.
- Section sequence and storytelling approach.
- Distinctive visual signature.
- Explicit list of common patterns intentionally avoided.

Do not reuse a previous project's full design identity, section order, hero composition, component arrangement, or visual signature by default.

### When building more than one website

If previous project context or existing project examples are available:
1. Inspect them for repeated visual patterns.
2. Identify the previous site's design fingerprint.
3. Deliberately choose a different composition, type pairing, image treatment, section rhythm, and interaction pattern where appropriate.
4. Reuse only neutral engineering foundations (accessibility helpers, utilities, tested components) when useful—not the previous site's complete art direction.

If no previous project context is available, do not claim knowledge of websites built for other users. Instead, maximize uniqueness within the current brief by deriving the design from the actual business, audience, references, assets, and goals. Do not invent a global uniqueness guarantee or claim access to other users' projects.

## Core principles

1. Understand the business before designing.
2. Inspect supplied references before implementation whenever tools permit.
3. Extract transferable principles, never copy a website.
4. Make a distinct creative direction for this business.
5. Establish a design system before assembling pages.
6. Make each section serve a user or business goal.
7. Build accessible, responsive, functional interfaces.
8. Run visual quality checks and iterate when tools permit.
9. Be honest about what was and was not inspected or tested.

## Workflow

### Phase 1 — Understand the brief

Inspect the existing project before changing it. Determine:
- Business category, business model, products/services.
- Target audience, market, and positioning.
- Primary conversion: purchase, booking, enquiry, visit, signup, call, etc.
- Required pages, content, integrations, and constraints.
- Existing framework, dependencies, assets, brand guidelines, and code conventions.
- Whether the user expects a new build or a redesign.

If one critical decision blocks progress, ask one concise question. Otherwise make sensible, reversible assumptions and state them briefly.

### Phase 2 — Inspect references

For every supplied URL:
1. Open the homepage and relevant inner pages.
2. Inspect first viewport and full-page structure when possible.
3. Check navigation, menus, buttons, forms, product/service discovery, and footer.
4. Check desktop and mobile widths when browser tools allow.
5. Separate directly observed facts from interpretation and assumptions.
6. Record access limitations honestly.

Use `references/reference-analysis.md` as the worksheet.

Study:
- Art direction and brand mood.
- Header/navigation behavior.
- Hero composition, copy density, media, and CTA.
- Typography scale, contrast, weight, line length.
- Color roles and contrast.
- Grid, whitespace, section rhythm, alignment.
- Photography/art direction and crop behavior.
- Product/service presentation.
- Trust signals and editorial storytelling.
- Interactions, motion, and responsive behavior.
- Conversion paths and friction.

Never claim exact fonts, CSS values, breakpoints, animation timings, or source implementation unless actually inspected. Visual estimates must be labeled as estimates.

### Phase 3 — Synthesize, do not imitate

Create a reference synthesis:
- Which principles are useful for this business?
- Which reference patterns are irrelevant?
- Which patterns conflict?
- What should be deliberately different?
- What is the original interpretation?

Do not combine every reference indiscriminately. Pick one coherent direction that fits the business. References are a source of inspiration and UX learning, not templates.

### Phase 4 — Create the Design Identity Record

Complete `references/uniqueness-protocol.md` before writing page components.

The record must be specific enough that another developer could distinguish this design from a generic template. Avoid vague descriptions like "modern, clean, premium". State concrete choices, for example:
- Asymmetric editorial split hero rather than centered hero.
- Full-bleed documentary photography rather than floating product mockups.
- Narrow serif display typography paired with neutral grotesk body text.
- Horizontal editorial product rail rather than uniform three-column cards.
- Warm paper-like surfaces and fine rules rather than glass panels and gradients.

These are examples only; do not reuse them automatically. Derive choices from the project.

### Phase 5 — Define the design system

Create tokens before page-level styling:
- Color roles: page, surface, text, muted text, border, brand, accent, CTA, semantic states.
- Typography: display, headings, body, UI; sizes, weights, line heights, tracking, fluid behavior.
- Layout: max width, gutters, grid, section spacing, responsive breakpoints.
- Shape: buttons, inputs, cards, dividers.
- Depth: shadows only when useful.
- Media: aspect ratios, object positioning, overlays, video behavior.
- Motion: duration, easing, distance, reduced-motion fallback.

Use CSS custom properties or the project's established token system. Do not force the same palette, font pairing, spacing scale, or component styling onto every business.

### Phase 6 — Plan the page architecture

Choose sections based on the business model and visitor intent. Possible sections:
- Announcement bar, if useful.
- Header and navigation.
- Hero with clear proposition and relevant imagery.
- Product/service/category discovery.
- Brand story or differentiators.
- Featured products, menu, services, collections, or locations.
- Process, experience, or how it works.
- Credible trust signals.
- Gallery/editorial content.
- FAQ when it removes real friction.
- Final CTA.
- Footer with useful contact, location, policies, and social links.

This is a pool of options, not a default sequence. Do not include every section. Avoid using the same section order on unrelated projects. Design the information architecture around the user's actual business and primary conversion.

### Phase 7 — Implement

- Respect the current stack and project architecture.
- Do not replace frameworks/tooling without a good reason.
- Use semantic HTML and accessible native controls.
- Use reusable components where they help; avoid over-componentization.
- Use responsive CSS and fluid layout where appropriate.
- Use supplied assets first. If assets are missing, use suitable licensed/stock assets or clearly marked placeholders.
- Never invent testimonials, addresses, awards, ratings, statistics, clients, opening hours, or business claims.
- Optimize images, avoid layout shifts, and lazy-load below-the-fold media.
- Ensure visible buttons and links have meaningful behavior.
- Implement forms, cart, booking, and integrations only to the level supported by the brief and available services. Never fake a successful transaction.
- Respect keyboard access, focus states, contrast, labels, heading order, and reduced motion.
- Keep dependencies and animations purposeful.

### Phase 8 — Anti-template visual review

Before completion, compare the result against:
1. The business brief.
2. The Design Identity Record.
3. Supplied references.
4. Any previous project examples available in the current context.

Ask:
- Could this exact page plausibly be used for a different business by swapping the logo and copy? If yes, it is too generic.
- Does the hero reflect this business's actual offer and audience?
- Is the section sequence business-specific?
- Are the imagery, type, composition, and interaction choices coherent?
- Have I repeated a common AI layout without a reason?
- Does the site have a memorable visual signature without copying a reference?

If it feels interchangeable, revise the concept and composition—not just the colors.

### Phase 9 — Visual quality assurance

When execution/browser tools are available:
- Run the application.
- Inspect wide desktop, laptop, tablet, and narrow mobile.
- Check first viewport, navigation, heading wraps, image crops, section rhythm, CTA paths, overflow, and interaction states.
- Check forms, errors, keyboard focus, and reduced motion.
- Check build/runtime errors where possible.
- Fix issues and repeat.

If visual inspection is unavailable, perform code-level checks and explicitly say visual QA was not completed.

## Anti-slop rules

Do not default to:
- Purple/blue gradients without a brand reason.
- Glassmorphism, glowing blobs, neon accents, or floating orbs as decoration.
- Generic centered hero with vague headline and two buttons.
- Repeated three-column feature-card sections.
- Rounded cards around every content block.
- Random icon grids, fake dashboards, fake stats, fake reviews, or invented press logos.
- Excessive pills, badges, borders, shadows, and gradients.
- Arbitrary scroll animations on every element.
- Lorem ipsum or placeholder copy left in the final result.
- Unrelated stock photography.

A clean design can still be expressive. Use distinctive composition, confident typography, considered imagery, strong hierarchy, and restrained details.

## Intellectual property and reference ethics

Use references to understand broad design approaches and common UX patterns. Do not copy source code, proprietary assets, logos, brand names, product photography, written copy, or distinctive trade dress. Do not reproduce a reference page pixel-for-pixel or imply affiliation with a reference brand.

Create original layouts and content for the user's business. If asked for a clone, offer a functionally similar but visually original implementation unless the user owns the source or has permission.

## Completion report

Summarize:
- Pages/sections implemented.
- Project-specific design direction.
- Key choices that make the result distinct.
- Functionality implemented and integrations still needed.
- Tests and viewport checks actually performed.
- Remaining limitations or placeholder assets.

Never claim global uniqueness across unrelated users or access to other users' work unless a real shared project registry or explicit cross-project context exists. Report only work actually completed.
