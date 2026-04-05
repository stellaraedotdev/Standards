# CSS Style Guide

## Architecture
- Use a consistent methodology for naming and composition.
- Keep selectors shallow and predictable.
- Prefer reusable utility and component patterns over one-off styles.

## Naming
- Use clear, descriptive class names.
- Avoid names tied to visual appearance alone when possible.
- Keep naming conventions consistent across the project.

## Specificity and Cascade
- Keep specificity low and manageable.
- Avoid `!important` except in tightly scoped utility cases.
- Use cascade layers or architecture conventions intentionally.

## Layout
- Prefer modern layout systems (`flex` and `grid`).
- Build responsive layouts mobile-first unless requirements differ.
- Use fluid spacing and sizing where practical.

## Variables and Theming
- Use CSS custom properties for shared tokens (color, spacing, radius, typography).
- Define tokens in a centralized theme layer.
- Avoid hard-coded repeated values.

## Performance
- Avoid expensive selectors and excessive overrides.
- Keep stylesheets organized and remove dead CSS.
- Minimize layout thrashing caused by JS-driven style changes.

## Accessibility
- Ensure sufficient color contrast.
- Preserve visible focus styles.
- Respect user preferences such as reduced motion.


## Rule Severity
- MUST: Mandatory requirement for consistency, safety, security, or correctness.
- SHOULD: Strong recommendation with limited exceptions when justified in the PR.
- MAY: Optional guidance that can improve quality when context allows.

## How to Use This Guide
- Apply these rules to new code by default.
- For existing code, improve areas you touch rather than broad unrelated rewrites.
- When a rule conflicts with product or platform constraints, document the exception and rationale.
- Prefer automated enforcement through formatters, linters, and CI checks.

## Pull Request Checklist
- Code follows naming, structure, and formatting conventions in this guide.
- Error handling and logging are explicit and appropriate.
- Tests were added or updated for changed behavior.
- Documentation was updated when behavior or developer workflow changed.
- Security, accessibility, and performance implications were considered.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
