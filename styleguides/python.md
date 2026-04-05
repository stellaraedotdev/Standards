# Python Style Guide

## Baseline
- Target Python version must be defined per project.
- Follow PEP 8 unless project tooling specifies stricter standards.
- Use automated formatting and linting in CI.

## Imports
- Group imports in this order: standard library, third-party, local.
- Avoid wildcard imports.
- Keep imports at module top unless lazy import is required.

## Naming
- Modules and variables: `snake_case`.
- Classes: `PascalCase`.
- Constants: `UPPER_SNAKE_CASE`.
- Private/internal members: leading underscore.

## Type Hints
- Use type hints for public APIs and non-trivial internal functions.
- Prefer built-in generic syntax (for supported Python versions).
- Keep annotations accurate during refactors.

## Functions and Classes
- Keep functions focused and side effects explicit.
- Prefer composition over deep inheritance trees.
- Use dataclasses for structured data when appropriate.

## Error Handling
- Catch specific exceptions, not broad `Exception`, unless re-raising with context.
- Include actionable messages in raised exceptions.
- Avoid using exceptions for expected control flow.

## Logging
- Use the `logging` module, not print statements, in application code.
- Use appropriate log levels (`debug`, `info`, `warning`, `error`, `critical`).
- Do not log secrets.

## Testing
- Use pytest unless project requirements differ.
- Prefer fixtures over duplicated setup code.
- Include tests for edge cases and error paths.

## Project Hygiene
- Pin or constrain dependencies responsibly.
- Keep `requirements` or equivalent dependency files updated.
- Document environment setup and common commands.


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
