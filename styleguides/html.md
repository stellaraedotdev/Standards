# HTML Style Guide

## Document Structure
- Use semantic HTML elements whenever possible.
- Include `<!doctype html>` and language declaration.
- Maintain a clear heading hierarchy (`h1` through `h6`).

## Semantics and Accessibility
- Use elements according to meaning, not appearance.
- Provide descriptive `alt` text for meaningful images.
- Associate form controls with labels.
- Ensure interactive elements are keyboard accessible.

## Attributes
- Use lowercase attribute names.
- Quote all attribute values.
- Keep IDs unique within the page.

## Content Organization
- Keep markup clean and intentionally nested.
- Avoid deeply nested div structures when semantic elements exist.
- Separate structure (HTML), presentation (CSS), and behavior (JS).

## Performance
- Load critical resources intentionally.
- Defer non-critical scripts when appropriate.
- Minimize unnecessary DOM complexity.

## Validation
- Validate HTML in CI or pre-release checks.
- Fix invalid markup promptly.


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
