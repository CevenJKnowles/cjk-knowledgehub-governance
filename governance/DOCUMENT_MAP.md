```yaml
id: GOV-MAP-00
layer: GOV
type: MAP
phase: X
status: active
created: 2026-02-16
updated: 2026-02-16
```
---
# DOCUMENT MAP — CJK KnowledgeHub Governance

This document defines the authoritative structure, routing logic, and control hierarchy of the `cjk-knowledgehub-governance` repository.

It governs:
- Folder semantics
- File placement rules
- Naming conventions
- Authority order
- Lifecycle transitions
- Structural invariants

If ambiguity arises regarding file placement or control precedence, this document is authoritative unless superseded by a newer ADR.

---

# 1. Authority Order

In case of conflict, the following precedence applies:

1. `MASTER_PROJECT_PROMPT.md`
2. `snapshots/SNP-CUR-01-current-state.md`
3. `control/*` (gates, DoD, QA rubric, architecture)
4. `governance/*` (ADRs, Intent Freezes, Project Brief)
5. `planning/*`
6. `execution/*`
7. `archive/*`

No file outside this order may override a higher authority layer.

---

# 2. Folder Semantics

## /governance
Purpose: Permanent structural law.

Contains:
- ADRs (Architecture Decision Records)
- Intent Freezes (P1–P4)
- Project Brief
- Deprecation Log
- This Document Map

Files in this directory define long-term rules and invariants.

---

## /control
Purpose: Operational enforcement layer.

Contains:
- Gates (GTE)
- Definition of Done (DOD)
- QA Rubrics (QAR)
- Phase Architecture Controls

These files determine whether a phase or artifact is allowed to progress.

---

## /planning
Purpose: Execution design and sequencing.

Contains:
- Workflow maps
- Strategy notes
- Phase planning documents

Planning files do not override governance or control.

---

## /snapshots
Purpose: State capture and resume safety.

Contains:
- Current active state
- Phase snapshots

Snapshots reflect status. They do not redefine structure.

---

## /execution
Purpose: Implementation artifacts and build outputs.

This directory contains artifacts produced during execution phases.

Execution files must conform to governance and control constraints.

---

## /data
Purpose: Reference material.

Contains:
- Background data
- Supporting context
- External references

Data files do not define structure.

---

## /archive
Purpose: Deprecated or superseded artifacts.

Archive is non-authoritative.
Files here are retained for traceability only.

---

# 3. Naming Convention Rules

Deterministic naming format:
PREFIX-CATEGORY-NUMBER-description.md

Examples:
- GOV-ADR-01-metadata-schema-v0-2.md
- CTL-GTE-02-p5-public-release-gate.md
- PLN-MAP-03-p5-prompt-projects.md

Rules:
- No spaces
- No dots in version slugs (use hyphen notation)
- Lowercase descriptive slugs
- Numeric sequencing required
- Prefix must match directory type

Exceptions must be explicitly defined in an ADR.

---

# 4. Routing Rules (Where Files Go)

| File Type | Location |
|-----------|----------|
| Architecture Decision Record | governance/ |
| Intent Freeze | governance/ |
| Gate | control/ |
| Definition of Done | control/ |
| QA Rubric | control/ |
| Workflow Map | planning/ |
| Strategy Note | planning/ |
| Snapshot | snapshots/ |
| Deprecated file | archive/ |
| Implementation artifact | execution/ |

If uncertain: default to `planning/` and escalate for structural review.

---

# 5. Lifecycle Transitions

Planning → Control Gate → Execution → Snapshot → Archive (if superseded)

Phases must pass defined Gates before transition.

Snapshots must be updated at:
- Phase completion
- Structural change
- Authority change

---

# 6. Structural Invariants

The following must always remain true:

- Deterministic naming
- Clear separation of governance vs planning
- Explicit authority hierarchy
- No silent structural drift
- Snapshot integrity maintained
- Archive never used as active reference

Violation of invariants requires an ADR.

---

# 7. Change Management

Structural changes require:

1. Proposal
2. Gate review
3. Snapshot update
4. ADR (if structural rule modified)

No structural change is considered valid until reflected in:
- Snapshot
- This Document Map (if affected)

---

# 8. Public Release Constraint (P5 Preparation)

Before public release:
- All entrypoints must resolve correctly
- Document Map must reflect actual structure
- No stub governance files allowed
- Naming conventions must be consistent
- Snapshot must be internally coherent

---

End of Document.
