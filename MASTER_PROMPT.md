---
id: GOV-POL-002
title: Master Project Prompt
type: pol
status: active
version: "2.0"
created: 2026-03-19
updated: 2026-03-19
provenance: ai-assisted
tags: [governance, master, policy, authority]
related: [TPL-001, INT-006, SNP-LOG-001]
ref: []
repo: []
---

# MASTER PROMPT
## CJK KnowledgeHub Governance Control System
Version: 2.0 — Supersedes DEP-MASTER_PROJECT_PROMPT_v1.md

---

## 1. Authority

This document is the single source of truth for governance rules inside:

`cjk-knowledgehub-governance`

No structural decision may violate this document.

If conflict arises, MASTER_PROMPT overrides all other files.

---

## 2. Naming Conventions

Two naming conventions coexist in this repository. Both are valid. They are distinguished by creation date.

### Legacy Convention (pre 2026-03-19)

```
[LAYER]-[TYPE]-[SEQ]-[SLUG].md
```

Example: `GOV-INT-01-p1-intent-freeze.md`

Applies to all files created before 2026-03-19. These files are not retroactively renamed.

### Current Convention (from 2026-03-19)

```
[TYPE]-[SEQ]-[slug].md
```

Example: `INT-006-knowledgehub-strategic-reset-intent-freeze.md`

Applies to all new files created from 2026-03-19 forward. Defined in full in [[TPL-001]].

### ID Format

The YAML `id` field is the canonical identity of every document. It is the anchor for all internal links. Format:

```
[TYPE]-[SEQ]
```

Example: `id: INT-006`

IDs never change. Slugs may be updated without breaking links.

### Root-Level Entrypoint Exception

The following root-level files are exempt from deterministic naming per GOV-ADR-02:

- `MASTER_PROMPT.md`
- `SESSION_PROMPT.md`
- `README.md`

The following governance index files are also exempt:

- `governance/DOCUMENT_MAP.md`
- `governance/DEPRECIATION_LOG.md`

---

## 3. Folder Structure

Allowed top-level folders:

```
/governance
/control
/planning
/execution
/snapshots
/data
/archive
```

No nested layer hierarchies unless explicitly frozen via ADR.

---

## 4. YAML Schema

All active files must begin with a YAML header. The canonical template is defined in [[TPL-001]].

Required fields:

```yaml
---
id: TYPE-001
title: Human readable title
type: type-code-lowercase
status: draft
version: "1.0"
created: YYYY-MM-DD
updated: YYYY-MM-DD
provenance: human | ai-assisted | ai-generated | session-derived
tags: []
related: []
ref: []
repo: []
---
```

No additional YAML keys unless frozen via ADR.

---

## 5. Layer Hierarchy (Authority Order)

```
governance > control > planning > execution > snapshots > data > archive
```

Higher layers override lower layers.

Snapshots record state. They do not define rules.

---

## 6. TYPE Registry (Frozen Vocabulary)

No new TYPE codes may be introduced without freezing via ADR.

### Governance (GOV / current: use TYPE only)

| Code | Meaning |
|---|---|
| `ADR` | Architecture Decision Record |
| `GOV` | Governance policy or rule |
| `INT` | Intent Freeze |
| `INV` | Invariant definition |
| `MAP` | Structural map |
| `POL` | Policy |
| `SCH` | Schema definition |

### Control

| Code | Meaning |
|---|---|
| `DOC` | Doctrine |
| `DOD` | Definition of Done |
| `QAR` | QA Rubric |
| `GTE` | Gate |

### Planning

| Code | Meaning |
|---|---|
| `PLN` | Plan or workflow map |
| `CHK` | Checklist |
| `KOF` | Kickoff |

### Snapshots

| Code | Meaning |
|---|---|
| `SNP` | Snapshot -- state capture |
| `LOG` | Session log |

### Execution

| Code | Meaning |
|---|---|
| `IMP` | Implementation |
| `BLD` | Build |
| `RUN` | Run log or execution record |

### Data

| Code | Meaning |
|---|---|
| `DAT` | Raw data or reference material |
| `IDX` | Index or registry |
| `TPL` | Template |

### Testing and Lab

| Code | Meaning |
|---|---|
| `INS` | Installation or first-run test |
| `LAB` | Lab notebook -- investigation |
| `TST` | Test document |

### Archive

| Code | Meaning |
|---|---|
| `DEP` | Deprecated (prefix only, not a TYPE code) |

---

## 7. Deprecation Protocol

Files are never deleted.

To deprecate:

1. Move file to `/archive/`
2. Prefix filename with `DEP-`
3. Update YAML `status: archived`
4. Add supersession notice at the top of the document body:

```markdown
> *Superseded by [[NEW-ID]] on YYYY-MM-DD.*
```

5. Log the deprecation in `governance/DEPRECIATION_LOG.md`

---

## 8. Status Lifecycle

```
draft > active > locked > archived
```

| Status | Meaning |
|---|---|
| `draft` | Being written. Not yet authoritative. |
| `active` | Authoritative. In effect. |
| `locked` | Stable. Changes require a new superseding document. |
| `archived` | Obsolete or superseded. Retained for traceability only. |

---

## 9. Freeze Rules

- Intent Freeze documents lock scope.
- ADR documents lock architecture.
- Doctrine documents lock implementation architecture.
- Definition of Done locks quality gates.
- QA Rubrics lock evaluation discipline.

Nothing bypasses a freeze without an explicit superseding document.

---

## 10. Vocabulary Expansion Rule

If a new TYPE, layer, or structural rule is needed:

1. Draft ADR.
2. Freeze via governance approval.
3. Update TYPE Registry.
4. Increment version.

No silent expansion.

---

## 11. Resume Safety Protocol

Every structural change must:

- Update `SNP-CUR-01-current-state.md`
- Update `DEPRECIATION_LOG.md` if applicable
- Preserve determinism
- Preserve traceability

No ambiguous states allowed.

---

## 12. Current Project State

**Project:** CJK KnowledgeHub Governance
**Active phase:** Phase 5 -- KnowledgeHub rebuild
**Authoritative freeze:** [[INT-006]]
**Session log:** [[SNP-LOG-001]]
**Naming convention:** [[TPL-001]]

Phase 5 objective: Full rebuild of the CJK KnowledgeHub under the AI Systems Architecture positioning confirmed in INT-006. Clean slate. Artefact-first information architecture.

---

*End of MASTER_PROMPT v2.0*
