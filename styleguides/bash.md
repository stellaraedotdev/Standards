# Bash Style Guide

## Baseline
- Start scripts with a clear shebang.
- Use `set -euo pipefail` for robust error behavior where appropriate.
- Keep scripts portable unless platform specificity is intentional and documented.

## Safety
- Quote variable expansions by default.
- Avoid unbounded globbing and unsafe word splitting.
- Validate inputs before executing commands.

## Structure
- Prefer functions for reusable logic.
- Keep scripts linear and easy to follow.
- Use descriptive variable and function names.

## Error Handling
- Exit with meaningful codes.
- Print actionable error messages to stderr.
- Handle expected failure modes explicitly.

## External Commands
- Check command availability when required.
- Prefer widely available tools.
- Avoid parsing human-oriented command output when machine formats exist.

## Logging
- Use concise, readable log messages.
- Distinguish informational output from errors.
- Never print secrets.

## Testing and Linting
- Run shellcheck for static analysis.
- Add tests for non-trivial scripts.
- Validate scripts in CI on target shells.


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
