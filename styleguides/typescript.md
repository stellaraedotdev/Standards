# TypeScript Style Guide

## Baseline
- Enable strict TypeScript settings for all production projects.
- Use project-wide formatting and linting in CI.
- Keep compiler options documented and intentional.

## Typing Principles
- Prefer explicit types for public APIs.
- Use type inference for obvious local variables.
- Avoid `any`; use `unknown` when type is not yet known.

## Interfaces and Types
- Use `interface` for object contracts likely to be extended.
- Use `type` for unions, intersections, and mapped or utility patterns.
- Keep types small and composable.

## Nullability
- Treat `null` and `undefined` intentionally.
- Narrow nullable values before use.
- Avoid non-null assertions (`!`) unless unavoidable and justified.

## Functions and APIs
- Keep function signatures focused and predictable.
- Prefer parameter objects when argument lists become long.
- Model errors and optional values explicitly in types.

## Enums and Literals
- Prefer string literal unions for many API contracts.
- Use `enum` only when runtime enum behavior is required.

## Imports and Modules
- Use consistent module resolution and path aliases.
- Keep import ordering consistent via tooling.
- Avoid importing from deep internal paths of third-party packages.

## Testing
- Type-check test code as well as source code.
- Add tests for type-sensitive logic and runtime behavior.
- Use fixtures and helpers to keep tests concise.


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
