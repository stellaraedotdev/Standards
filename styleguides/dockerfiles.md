# Dockerfiles Style Guide

## Base Images
- Use minimal, trusted base images.
- Pin image tags to predictable versions.
- Prefer official images where feasible.

## Build Strategy
- Use multi-stage builds for smaller production images.
- Keep layers intentional and cache-friendly.
- Place frequently changing steps later when practical.

## Security
- Run as non-root unless a clear exception is documented.
- Minimize installed packages and attack surface.
- Do not bake secrets into images.

## Reproducibility
- Pin package versions when practical.
- Keep build inputs explicit.
- Record required build arguments and defaults.

## Readability
- Group related instructions logically.
- Use clear comments sparingly for non-obvious decisions.
- Keep Dockerfiles focused and maintainable.

## Runtime Behavior
- Use `CMD` and `ENTRYPOINT` intentionally.
- Prefer exec form for process signal handling.
- Define health checks when they provide meaningful value.

## Validation
- Build images in CI.
- Scan images for vulnerabilities regularly.
- Remove deprecated or unused images and tags.


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
