# JSON Style Guide

## Formatting
- Use spaces for indentation, with a consistent width per project.
- Keep key order stable when readability benefits from it.
- Use UTF-8 encoding.

## Data Modeling
- Keep schema explicit and versioned when used externally.
- Use arrays and objects consistently for predictable parsing.
- Avoid polymorphic structures unless clearly documented.

## Keys and Values
- Use descriptive and stable key names.
- Keep naming conventions consistent across payloads.
- Prefer explicit `null` handling rules in schema documentation.

## Safety and Compatibility
- Avoid trailing commas and comments in strict JSON.
- Validate payloads against schema where practical.
- Handle unknown fields safely in consumers.

## Size and Performance
- Keep payloads focused and minimal.
- Avoid deeply nested structures that harm readability and parsing.
- Compress or paginate large payloads where required.

## Validation and Testing
- Validate JSON in CI for syntax and schema conformance.
- Include contract tests for producer-consumer boundaries.
- Track schema changes with clear migration guidance.


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
