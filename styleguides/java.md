# Java Style Guide

## Baseline
- Use the project-defined Java version consistently.
- Enforce formatting, linting, and static analysis in CI.
- Keep build configuration reproducible and explicit.

## Naming
- Classes and interfaces: `PascalCase`.
- Methods and variables: `camelCase`.
- Constants: `UPPER_SNAKE_CASE`.
- Package names: lowercase and domain-structured.

## Class Design
- Keep classes focused on a single responsibility.
- Favor composition over inheritance where possible.
- Limit mutable state and expose clear invariants.

## Null Handling
- Avoid returning `null` when alternatives are available.
- Use `Optional` for return values where semantically appropriate.
- Validate constructor and method inputs early.

## Exceptions
- Throw specific exceptions with actionable messages.
- Avoid broad catch blocks that hide root causes.
- Preserve original exception context when wrapping.

## Collections and Streams
- Use interfaces (`List`, `Map`) for abstractions.
- Prefer immutable or unmodifiable collections for shared data.
- Keep stream pipelines readable; avoid over-complex chaining.

## Testing
- Write unit tests for behavior and edge cases.
- Use integration tests for cross-boundary behavior.
- Keep tests deterministic and independent.


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
