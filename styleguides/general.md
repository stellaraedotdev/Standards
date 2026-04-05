# General Style Guide

## Purpose
This document defines baseline standards that apply to all languages and repositories.

## Core Principles
- Prefer readability over cleverness.
- Keep code and documentation simple, explicit, and maintainable.
- Optimize for long-term ownership, not short-term speed.
- Make behavior predictable and easy to test.

## Naming
- Use clear, intention-revealing names.
- Avoid ambiguous abbreviations unless they are widely understood.
- Keep naming consistent within each module and across the project.

## Structure
- Keep files focused on a single responsibility.
- Keep functions and methods small and cohesive.
- Separate pure logic from I/O and side effects when practical.

## Formatting
- Use project formatters and linters consistently.
- Keep line lengths reasonable for readability.
- Use whitespace intentionally to separate concerns.

## Comments
- Write comments that explain why, not what.
- Remove stale comments promptly.
- Prefer self-explanatory code over excessive commentary.

## Error Handling
- Fail fast with clear, actionable error messages.
- Do not silently ignore errors.
- Handle expected failures close to their source.

## Logging
- Log meaningful events and errors.
- Never log secrets or sensitive user data.
- Use structured logging where available.

## Dependencies
- Add dependencies only when justified.
- Prefer mature, well-maintained libraries.
- Remove unused dependencies quickly.

## Testing Expectations
- Add or update tests for behavior changes.
- Test critical paths and edge cases.
- Keep tests deterministic and isolated.

## Documentation
- Keep docs close to the code they describe.
- Update docs in the same change as behavior updates.
- Favor examples for complex workflows.

## Review Readiness
- Ensure changes are small enough to review effectively.
- Include context, rationale, and known trade-offs.
- Verify linting, tests, and build checks before requesting review.


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
