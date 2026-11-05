# Workflow: implement and review

1. Inspect the existing source tree and package configuration.
2. Preserve the current stack unless the user requests otherwise or a change is justified.
3. Implement semantic structure and responsive layout.
4. Add the design tokens and reusable components.
5. Wire all visible controls to real behavior or mark integrations that need credentials/backend support.
6. Run the development server/build using the project's existing commands.
7. Inspect screenshots at wide desktop, laptop, tablet, and mobile widths when browser tools are available.
8. Fix layout, typography, crop, overflow, contrast, and interaction issues.
9. Check keyboard access, focus states, labels, and reduced motion.
10. Re-run checks after fixes.
11. Report exactly what was implemented and tested.

Do not say "fully responsive", "production-ready", or "tested" unless the relevant checks were actually performed. Distinguish code-level review from browser-based visual QA.
