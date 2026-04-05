# C Style Guide

## Baseline
- Target C standard must be declared per project.
- Compile with warnings enabled and treat warnings as errors where feasible.
- Use formatting and static analysis tools consistently.

## Naming
- Use descriptive names with project-consistent casing.
- Prefix global symbols to avoid collisions.
- Use `UPPER_SNAKE_CASE` for macros and constants.

## Header and Source Organization
- Keep declarations in headers and definitions in source files.
- Use include guards or `#pragma once` consistently.
- Minimize header dependencies.

## Memory Management
- Make ownership rules explicit.
- Pair allocations and deallocations clearly.
- Initialize memory before use and avoid leaks.

## Safety
- Validate external inputs.
- Check bounds on buffer operations.
- Prefer safer standard library patterns and wrappers where available.

## Error Handling
- Return clear status codes and document them.
- Check all critical function return values.
- Centralize cleanup paths to avoid leaks in error branches.

## Testing
- Add tests for boundary conditions and failure paths.
- Use sanitizers in CI when available.
- Include regression tests for bug fixes.


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
