# Documentation Guidelines

## Purpose
Ensure documentation is accurate, maintainable, and useful to both new and experienced contributors.

## Scope
Covers product documentation, developer documentation, architecture notes, runbooks, and inline usage docs.

## Core Principles
- Documentation is part of the product and must be maintained with code.
- Prefer clear, direct language over exhaustive but ambiguous wording.
- Optimize for discoverability and task completion.

## Required Document Structure
- Start with purpose and intended audience.
- Include prerequisites and environment assumptions.
- Provide step-by-step procedures for operational tasks.
- Include troubleshooting for common failures.
- Include ownership and last-updated metadata when applicable.

## Writing Standards
- Use consistent terminology across repositories.
- Define acronyms on first use.
- Use active voice and concise sentences.
- Prefer examples for complex configuration or workflows.

## Code and Command Examples
- Ensure examples are copy-paste ready.
- Use realistic values and clearly mark placeholders.
- Keep examples tested against current behavior.
- Explain non-obvious flags and options.

## Update Policy
- Update documentation in the same pull request as behavior changes.
- Remove or fix stale docs immediately when discovered.
- Add migration notes for breaking changes.

## Quality Gates
- Validate internal and external links regularly.
- Lint markdown in CI where possible.
- Require review for correctness and clarity on major docs.

## Operational Documentation
- Keep runbooks actionable under incident pressure.
- Include rollback and recovery procedures.
- Include clear escalation paths and contact points.

## Rule Severity
- MUST: Required for correctness and maintainability.
- SHOULD: Expected unless there is a documented reason not to.
- MAY: Helpful additions that improve comprehension.

## Pull Request Checklist
- Docs match current behavior.
- Examples and commands are verified.
- New terminology is defined.
- Links and references are valid.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
