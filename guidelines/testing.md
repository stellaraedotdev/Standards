# Testing Guidelines

## Purpose
Establish consistent test practices that prevent regressions, protect critical paths, and support safe delivery.

## Scope
Applies to unit, integration, end-to-end, contract, performance, and security-related automated tests.

## Test Strategy
- Use the test pyramid as a default: more unit tests, fewer end-to-end tests.
- Place tests close to the behavior they validate.
- Prioritize tests for business-critical and high-risk paths.

## Required Coverage Expectations
- Every behavior change must include or update tests.
- Every bug fix must include a regression test.
- High-risk modules should include boundary and failure-case coverage.

## Test Quality Standards
- Tests must be deterministic and isolated.
- Avoid shared mutable global state in tests.
- Use clear test names that describe expected behavior.
- Prefer explicit setup over hidden fixtures for critical flows.

## Integration and Contract Testing
- Validate interfaces between services and components.
- Use contract tests for API compatibility.
- Include negative-path tests for invalid inputs and failure responses.

## End-to-End Testing
- Keep end-to-end tests focused on core user journeys.
- Minimize flakiness through stable selectors and robust waits.
- Quarantine flaky tests only with a tracked remediation issue.

## CI and Release Gates
- Run required test suites in CI for every pull request.
- Block merges on failing required tests.
- Track test duration and optimize bottlenecks regularly.

## Test Data and Security
- Do not use real sensitive production data in tests.
- Sanitize fixtures and snapshots.
- Rotate secrets used in test environments according to policy.

## Rule Severity
- MUST: Required for merge readiness and release safety.
- SHOULD: Strongly recommended for reliability and speed.
- MAY: Optional improvements for confidence or maintainability.

## Pull Request Checklist
- Changed behavior has automated coverage.
- Regression tests added for fixed bugs.
- Flaky tests were not introduced.
- CI test results are green.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
