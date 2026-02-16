---
id: GOV-POL-01
layer: GOV
type: POL
phase: X
status: active
created: 2026-02-16
updated: 2026-02-16
---
---
# MASTER_PROJECT_PROMPT
## CJK KnowledgeHub Governance Control System
Version: 1.0 (Frozen)

---

# 1. Authority

This document is the single source of truth for governance rules inside:

cjk-knowledgehub-governance

No structural decision may violate this document.

If conflict arises:
MASTER_PROJECT_PROMPT overrides all other files.

---

# 2. Deterministic Naming Convention

All files must follow:

[LAYER]-[TYPE]-[SEQ]-[SLUG].md

Example:
GOV-INT-01-p1-intent-freeze.md

ID format (immutable):
[LAYER]-[TYPE]-[SEQ]

The SLUG is descriptive but non-authoritative.
The ID is the authoritative identity.

IDs never change.

---

# 3. Folder Structure (Flat Per Layer)

Allowed top-level folders:

/governance
/control
/planning
/execution
/snapshots
/data
/archive

No nested layer hierarchies unless explicitly frozen via ADR.

---

# 4. YAML Schema (Frozen)

All active files must begin with:

---

## YAML Template (example only)

```yaml
text
layer_example: <layer>
type_example: <type>
phase_example: <number or X>
```
No additional YAML keys unless frozen via ADR.

---

# 5. Layer Hierarchy (Authority Order)

governance > control > planning > execution > snapshots > data > archive

Higher layers override lower layers.

Snapshots record history.
They do not define rules.

---

# 6. TYPE Registry (Frozen Vocabulary)

No new TYPE codes may be introduced without freezing vocabulary via ADR.

## 6.1 Governance (GOV)

INT  — Intent Freeze  
ADR  — Architecture Decision Record  
MAP  — Structural Map  
POL  — Policy  
SCH  — Schema  

## 6.2 Control (CTL)

DOC  — Doctrine  
DOD  — Definition of Done  
QAR  — QA Rubric  
GTE  — Gate  

## 6.3 Planning (PLN)

PLN  — Plan  
CHK  — Checklist  
MAP  — Structural Map  
KOF  — Kickoff  

## 6.4 Execution (EXE)

IMP  — Implementation  
BLD  — Build  
RUN  — Run Log  

## 6.5 Snapshot (SNP)

CUR  — Current State  
PHS  — Phase Snapshot  
LOG  — Log  

## 6.6 Data (DAT)

CVP  — CV Payload  
LNK  — Link Registry  
RAW  — Raw Data  
REF  — Reference  

## 6.7 Archive (ARC)

DEP  — Deprecated

---

# 7. Deprecation Protocol

Files are never deleted.

To deprecate:

1. Move to /archive
2. Prefix filename with: DEP-
3. Update YAML:
   status: deprecated
4. Add banner at top:

# ⚠ Deprecated
Superseded by: <New File>
Date: YYYY-MM-DD

All deprecations must be logged in:

governance/DEPRECIATION_LOG.md

---

# 8. Freeze Rules

- Intent Freeze documents lock scope.
- ADR documents lock architecture.
- Doctrine documents lock implementation architecture.
- Definition of Done locks quality gates.
- QA Rubrics lock evaluation discipline.

Nothing bypasses a freeze without explicit superseding document.

---

# 9. Vocabulary Expansion Rule

If a new TYPE, layer, or structural rule is needed:

1. Draft ADR.
2. Freeze via governance approval.
3. Update TYPE Registry.
4. Increment version.

No silent expansion.

---

# 10. Resume Safety Protocol

Every structural change must:

- Update CURRENT_STATE.md
- Update DEPRECIATION_LOG if applicable
- Preserve determinism
- Preserve traceability

No ambiguous states allowed.

---

End of MASTER_PROJECT_PROMPT

