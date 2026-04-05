# XML Style Guide

## Structure
- Keep XML documents well-formed and valid against schema or DTD when required.
- Use a clear element hierarchy with meaningful names.
- Avoid unnecessary nesting.

## Naming and Namespaces
- Use consistent element and attribute naming conventions.
- Declare and use namespaces explicitly when integrating multiple vocabularies.
- Avoid ambiguous prefixes.

## Attributes vs Elements
- Use attributes for metadata and concise properties.
- Use elements for structured or repeatable content.
- Apply this rule consistently across the document model.

## Formatting
- Use consistent indentation and line breaks.
- Keep long text content readable.
- Preserve canonical ordering when required by downstream systems.

## Validation
- Validate against XSD where schemas are available.
- Enforce validation in CI for contract-critical XML.
- Version schemas and communicate breaking changes.

## Security
- Disable external entity resolution unless explicitly required and controlled.
- Sanitize untrusted input before parsing.
- Avoid exposing sensitive data in serialized XML.


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
