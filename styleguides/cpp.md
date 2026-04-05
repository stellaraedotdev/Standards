# C++ Style Guide

## Baseline
- Target C++ standard must be defined per project.
- Use consistent formatting and static analysis in CI.
- Prefer compiler warnings at high strictness.

## Naming
- Use consistent naming conventions project-wide.
- Types should be clearly distinguishable from variables and functions.
- Constants should be obvious and immutable by design.

## Resource Management
- Prefer RAII for all resource ownership.
- Use smart pointers instead of raw owning pointers.
- Avoid manual `new` and `delete` in application code.

## APIs and Types
- Prefer value semantics where practical.
- Mark single-argument constructors `explicit`.
- Use `const` correctness consistently.

## Modern C++ Practices
- Prefer `std::array`, `std::vector`, and standard containers.
- Prefer standard algorithms over manual loops when clearer.
- Use `auto` where type is obvious or verbose.

## Error Handling
- Use exceptions or error-return patterns consistently per project policy.
- Maintain strong invariants and document assumptions.
- Avoid swallowing errors silently.

## Testing
- Cover edge cases and ownership-sensitive behavior.
- Use sanitizers and static analysis in CI.
- Add regression tests with every bug fix.


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
