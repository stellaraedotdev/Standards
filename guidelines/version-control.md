# Version Control Guidelines

## Purpose
Define version control practices that maintain clean history, safe collaboration, and reliable releases.

## Scope
Applies to branching, commits, pull requests, rebasing, merging, tagging, and release maintenance.

## Branching Model
- Keep a protected default branch for releasable code.
- Use short-lived feature branches for active work.
- Use release branches only when release processes require them.
- Delete merged branches promptly.

## Commit Standards
- Keep commits atomic and focused on one logical change.
- Use clear commit messages with intent and impact.
- Prefer multiple small commits over one large opaque commit.
- Do not commit generated artifacts unless repository policy requires it.

## History Hygiene
- Rebase or merge frequently to reduce long-lived drift.
- Avoid force-pushing shared branches unless coordinated.
- Preserve useful context in commit history for future debugging.

## Merge Policy
- Merge only through pull requests.
- Require passing checks and approved reviews before merge.
- Use merge methods that preserve readability and traceability.

## Tags and Releases
- Use annotated tags for releases.
- Follow a documented versioning strategy.
- Include release notes with notable changes and migration guidance.

## Access and Protection
- Protect default and release branches with rules.
- Restrict direct pushes to protected branches.
- Enforce signed commits or signatures where required by policy.

## Incident and Hotfix Flow
- Document hotfix branching and backport procedures.
- Ensure hotfixes receive post-incident review.
- Synchronize fixes across supported branches.

## Rule Severity
- MUST: Required controls for repository integrity.
- SHOULD: Strong conventions for maintainable history.
- MAY: Optional optimizations for team workflow.

## Pull Request Checklist
- Branch and commit scope are focused.
- Required checks and reviews are complete.
- Versioning and release notes are updated when needed.
- Protected branch policies were respected.

<sub>&copy; 2026 Stellarae | Documents licensed under MIT License. Treat the documents outlined here as 'the Software' in terms of the license.</sub>
