# Code Reviews Guidelines

## Purpose
Set review standards that improve code quality, reduce risk, and share knowledge efficiently.

## Scope
Applies to all pull requests, including code, tests, docs, infrastructure, and configuration changes.

## Review Objectives
- Verify correctness against requirements.
- Identify risks in security, privacy, accessibility, and performance.
- Ensure maintainability, readability, and testability.
- Confirm adequate tests and documentation updates.

## Author Responsibilities
- Keep pull requests focused and reviewable.
- Provide context, design rationale, and risk notes.
- Include test evidence and screenshots where applicable.
- Respond to feedback constructively and promptly.

## Reviewer Responsibilities
- Review for behavior, risks, and long-term maintainability first.
- Be specific, actionable, and respectful in feedback.
- Differentiate blocking issues from suggestions.
- Verify critical comments are resolved before approval.

## Review Depth by Change Risk
- Low risk: Quick validation with spot checks and test confirmation.
- Medium risk: Full diff review with targeted scenario verification.
- High risk: Deep review, multi-reviewer approval, and rollout safeguards.

## Required Checks During Review
- Requirements are satisfied and edge cases considered.
- Error handling and observability are adequate.
- Tests cover changed and failure behavior.
- Public interfaces and docs are updated where needed.

## Turnaround and Collaboration
- Prioritize review queues to reduce lead time.
- Escalate blocked reviews quickly.
- Resolve major architectural disagreements through design discussion.

## Rule Severity
- MUST: Blocking quality or risk concern that must be resolved.
- SHOULD: Important improvement that is expected unless justified.
- MAY: Optional suggestion for readability or consistency.

## Pull Request Checklist
- Review scope and risk were assessed.
- Blocking comments were resolved.
- Tests and docs updates were verified.
- Final approval reflects the current diff state.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
