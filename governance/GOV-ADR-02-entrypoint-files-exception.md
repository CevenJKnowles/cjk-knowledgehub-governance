---
id: GOV-ADR-02
layer: GOV
type: ADR
phase: X
status: active
created: 2026-02-16
updated: 2026-02-16
---
---
# ADR-02 — Entrypoint Files Exception (Root-Level Meta Files)

## Decision

The following files are allowed to remain in the repository root and are exempt from the deterministic filename convention:

- MASTER_PROJECT_PROMPT.md
- SESSION_PROMPT.md
- README.md

The following governance indexes are allowed to remain in `governance/` with human-readable names and are exempt from deterministic filename convention:

- governance/DOCUMENT_MAP.md
- governance/DEPRECIATION_LOG.md

## Rationale

These files function as *entrypoint/meta* documents for fast orientation and drift prevention.

- They are intended to be read first.
- Their human-readable names improve discoverability.
- They serve as stable anchors for both human and assistant navigation.

## Constraints

1. This exception applies only to the explicit filenames listed above.
2. No additional exceptions may be added without a new ADR.
3. These files must still comply with the frozen YAML schema and vocabulary where applicable.
4. All other files must follow:
   `[LAYER]-[TYPE]-[SEQ]-[SLUG].md`

## Consequences

- Root-level clarity improves onboarding and reduces mis-navigation.
- Determinism remains intact for all other artifacts.
- Exception scope is bounded and auditable via ADR.
