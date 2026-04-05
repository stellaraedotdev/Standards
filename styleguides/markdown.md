# Markdown Style Guide

## Purpose
- Write documentation that is clear, scannable, and actionable.
- Optimize for maintainability and long-term readability.

## Structure
- Use one `#` title per document.
- Use logical heading hierarchy without skipping levels.
- Keep sections concise and focused.

## Writing Style
- Prefer plain language and direct sentences.
- Use consistent terminology across documents.
- Avoid unnecessary jargon and ambiguity.

## Lists and Examples
- Use bullets for unordered concepts and numbered lists for sequences.
- Keep list item style consistent within a section.
- Include runnable or realistic examples where useful.

## Code and Commands
- Use fenced code blocks with language tags.
- Keep command examples copy-paste ready.
- Explain non-obvious flags or parameters.

## Links and References
- Prefer relative links for repository-local references.
- Keep link text descriptive.
- Regularly validate links and anchors.

## Tables and Callouts
- Use tables only when they improve comparison clarity.
- Keep table content short and readable.
- Use consistent callout patterns for warnings and notes.

## Maintenance
- Update docs alongside behavior changes.
- Remove outdated sections promptly.
- Track major documentation changes in version history when needed.


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
