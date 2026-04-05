# YAML Style Guide

## Formatting
- Use spaces for indentation; never use tabs.
- Keep indentation width consistent within a file.
- Use UTF-8 and Unix line endings unless project policy differs.

## Structure
- Keep documents shallow and readable.
- Use sequences and mappings consistently.
- Avoid unnecessary nesting and duplication.

## Keys and Values
- Use clear, stable key names.
- Keep key casing consistent project-wide.
- Quote values when ambiguity is possible.

## Anchors and Aliases
- Use anchors and aliases sparingly.
- Prefer explicit duplication over hard-to-follow indirection.
- Document complex anchor usage.

## Environment and Secrets
- Do not commit secrets in YAML files.
- Reference secrets through approved secret management systems.
- Validate required environment values in CI.

## Validation
- Lint and validate schema in CI where applicable.
- Fail fast on invalid structure.
- Keep examples aligned with actual schema behavior.


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
