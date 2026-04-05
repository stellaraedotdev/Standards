# Rust Style Guide

## Baseline
- Track and document the minimum supported Rust version (MSRV).
- Enforce formatting with `rustfmt` and linting with `clippy`.
- Keep warnings treated as actionable work.

## Naming
- Types and traits: `PascalCase`.
- Functions, variables, modules: `snake_case`.
- Constants and statics: `UPPER_SNAKE_CASE`.

## Ownership and Borrowing
- Prefer borrowing over cloning when practical.
- Keep lifetimes explicit only when inference is insufficient.
- Minimize mutable state and mutation scope.

## Error Handling
- Use `Result` for recoverable errors and `panic!` only for unrecoverable invariants.
- Define clear error types for library boundaries.
- Add context when propagating errors.

## API Design
- Keep public APIs small and intention-revealing.
- Prefer iterators and zero-cost abstractions.
- Avoid exposing internal implementation details.

## Concurrency
- Prefer message passing or clear synchronization primitives.
- Avoid shared mutable state unless necessary.
- Document thread-safety assumptions for public types.

## Testing
- Include unit tests near implementation and integration tests when needed.
- Test edge cases and failure modes.
- Keep tests deterministic.


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
