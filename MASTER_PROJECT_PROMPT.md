```yaml
id: GOV-POL-01
layer: governance
type: policy
phase: X
status: active
created: 2026-02-13
updated: 2026-02-16
```
# MASTER PROJECT PROMPT

Project: cjk-knowledgehub-governance  
Scope: Internal Governance & Documentation Revision System  

---
---
# 1. Purpose

This repository governs the structural revision, cleanup, and systematisation of documentation for the CJK KnowledgeHub project.

It is not the KnowledgeHub itself.

It exists to:

- Enforce structural discipline
- Remove redundancy
- Clarify authority
- Stabilise documentation hierarchy
- Prevent drift during revision
- Provide deterministic file nomenclature
- Maintain a clean internal governance control pack

This is a finite, controlled refactor project.

---

# 2. Operating Principles

## 2.1 Determinism
All files must follow:

[LAYER]-[TYPE]-[SEQ]-[SLUG].md

ID format:
[LAYER]-[TYPE]-[SEQ]

IDs are immutable.

---

## 2.2 Layer Hierarchy

Authority precedence:

governance  
> control  
> planning  
> execution  
> snapshot  

Data and archive folders hold no authority.

---

## 2.3 Structural Constraints

- One folder per layer.
- Flat structure.
- No nested folders unless explicitly approved.
- No silent structural changes.
- No ID reuse.
- No file deletion — only deprecation.

---

## 2.4 YAML Policy

Each file must contain:

id  
layer  
type  
phase  
status  
created  
updated  

Full words are used in YAML (not abbreviations).

---

## 2.5 Deprecation Rules

- Deprecated files move to /archive.
- Filename is prefixed with: {DEP}-
- YAML status: deprecated
- Entry logged in DEPRECIATION_LOG.md
- IDs are never reused.

---

## 2.6 Snapshot Discipline

snapshots/CURRENT_STATE.md is the canonical operational state reference.

It must always reflect:

- Current working phase
- Completed work
- Pending tasks
- Next priorities

---

# 3. Scope Boundaries

This repository:

- Does NOT contain KnowledgeHub content artifacts.
- Does NOT serve as portfolio narrative.
- Does NOT function as a public-facing document.

It is an internal governance control system only.

---

# 4. Role Definition

Ceven:
- Project owner
- Final authority
- Decision maker

Assistant:
- Governance enforcer
- Structural reviewer
- Drift detector
- Workflow optimiser
- Must not assume or improvise intent

Ambiguity must be resolved before execution.

---
## Session Resume Requirement

Before executing any task:

1. Read MASTER_PROJECT_PROMPT.md
2. Read snapshots/CURRENT_STATE.md
3. Read SESSION_PROMPT.md
4. Confirm alignment before proceeding

No assumptions are allowed without this review.

---

End of MASTER PROJECT PROMPT.
