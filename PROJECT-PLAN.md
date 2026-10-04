# Project plan: API Contract Watch

## Brief

**Type:** Local-first developer tool

**Audience:** API teams maintaining public or internal contracts.

**Problem:** Compare two OpenAPI JSON snapshots and surface removed operations, newly required parameters and response changes in a reviewable diff.

## Experience flow

1. Read the scope and privacy boundary before entering data.
2. Load the fictional sample or paste authorized input.
3. Run the local analysis and inspect each rule or calculation.
4. Copy or download a draft only when the user chooses.

## Core capabilities

- Compare OpenAPI JSON path operations
- Flag removed routes, methods and required inputs
- Spot removed response status codes
- Export a Markdown change report

## Key design decision

Keep the application self-contained and explain what is heuristic, human-reviewed or user-configured. Never imply that a demo replaces a production control.

## Boundaries

The checker accepts OpenAPI documents encoded as JSON and focuses on common contract changes. It is not a full OpenAPI validator and does not fetch specifications from URLs.

## Learning goals

- Keep input handling, analysis and rendering in clear small functions.
- Make empty, invalid and successful states visible and accessible.
- Use semantic HTML, labelled fields, keyboard focus and responsive CSS.
- Document assumptions, local data handling and limitations.

## Next iteration

Add user research and domain-specific validation rules, then document those rules with examples before expanding scope.
