# Project Structure Guidelines

## Purpose
Define repository structure patterns that improve discoverability, onboarding speed, and long-term maintainability.

## Scope
Applies to single-service repositories, monorepos, libraries, and tooling repositories.

## Core Principles
- Organize by domain and responsibility, not by technical artifact alone.
- Keep top-level directories minimal and intentional.
- Make common paths predictable across repositories.

## Recommended Top-Level Layout
- src: Application or library source code.
- tests: Automated tests when not colocated.
- docs: Product, architecture, and operational documentation.
- scripts: Automation scripts for development and release workflows.
- config: Non-secret configuration templates and schemas.

## Module Boundaries
- Define clear ownership and responsibilities per module.
- Minimize cross-module coupling and cyclic dependencies.
- Expose stable interfaces and keep internals private by default.

## Naming and Placement
- Use consistent naming conventions for files and directories.
- Keep related files close together.
- Avoid deep nesting that hides core workflows.

## Configuration and Environment
- Separate environment-specific configuration from source code.
- Keep secrets out of the repository.
- Document required environment variables and defaults.

## Build and Tooling Organization
- Keep build, lint, test, and release scripts discoverable.
- Centralize shared tooling config where practical.
- Avoid duplicating workflow definitions across modules.

## Documentation and Ownership
- Include a clear README at repository root.
- Add module-level READMEs for complex areas.
- Document ownership for critical directories.

## Rule Severity
- MUST: Required for maintainable structure and safe collaboration.
- SHOULD: Strong conventions for consistency and onboarding.
- MAY: Optional patterns for specific team workflows.

## Pull Request Checklist
- New files are placed in appropriate directories.
- Module boundaries and ownership remain clear.
- Config and environment changes are documented.
- README and architecture notes are updated when needed.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
