# Go Style Guide

## Baseline
- Follow standard Go formatting with `gofmt`.
- Use `go vet` and linters in CI.
- Keep module dependencies tidy and minimal.

## Naming
- Use short, clear names with package context in mind.
- Exported identifiers use `PascalCase`; unexported use `camelCase`.
- Avoid stutter in names (for example, `user.Service`, not `user.UserService`).

## Package Design
- Keep packages focused and cohesive.
- Avoid cyclic dependencies.
- Prefer small interfaces defined by consumers.

## Error Handling
- Return errors as values and check them immediately.
- Wrap errors with context where useful.
- Do not ignore returned errors unless explicitly safe.

## Concurrency
- Use goroutines intentionally and avoid leaks.
- Coordinate with channels and context cancellation.
- Document ownership and lifecycle of background workers.

## Context Usage
- Accept `context.Context` as first parameter for request-scoped operations.
- Do not store contexts in structs.
- Honor cancellation and deadlines.

## Testing
- Write table-driven tests for variant behavior.
- Use subtests where it improves clarity.
- Keep tests isolated and deterministic.


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
