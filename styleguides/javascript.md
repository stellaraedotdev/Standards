# JavaScript Style Guide

## Baseline
- Use modern ECMAScript features supported by the runtime target.
- Enforce style with formatter and linter in CI.
- Prefer strict mode behavior through tooling and language settings.

## Declarations
- Use `const` by default.
- Use `let` when reassignment is required.
- Avoid `var`.

## Naming
- Variables and functions: `camelCase`.
- Classes and constructors: `PascalCase`.
- Constants: `UPPER_SNAKE_CASE` when semantically constant.

## Functions
- Prefer small, pure functions where practical.
- Use arrow functions for short callbacks.
- Avoid deeply nested callback chains; prefer `async` and `await`.

## Async Code
- Handle promise failures explicitly.
- Avoid unawaited promises unless intentionally fire-and-forget and documented.
- Use `Promise.all` for independent concurrent operations.

## Objects and Arrays
- Favor immutable updates when working with shared state.
- Use destructuring for clarity when it improves readability.
- Avoid mutating function inputs unless documented.

## Error Handling
- Throw `Error` objects, not raw strings.
- Include contextual details in errors.
- Surface recoverable errors to callers cleanly.

## Modules
- Prefer ES modules unless platform constraints require otherwise.
- Keep module boundaries clear and cohesive.
- Avoid circular dependencies.

## Testing
- Write tests for changed behavior and regressions.
- Test both happy paths and failure paths.
- Keep tests independent and deterministic.


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
