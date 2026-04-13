---
id: TPL-001
title: CJK Unified Naming Convention System
type: tpl
status: locked
version: "2.0"
created: 2026-03-19
updated: 2026-04-13
provenance: ai-assisted
tags: [governance, naming, convention, yaml, zettlr]
related: [LOG-001]
ref: []
repo: []
---

# CJK Unified Naming Convention System

---

## 1. Purpose

This document defines the canonical naming convention, YAML schema, and TYPE code registry for all new documents created by Ceven Jupiter Knowles from 2026-03-19 forward.

It applies across all repos and knowledge environments including JupyterLab, Zettlr, MkDocs, and GitHub.

It does not retroactively rename existing documents.

---

## 2. Core Decisions

| # | Decision |
|---|---|
| 1 | No repo identifier in filename |
| 2 | Date in YAML only. Fields: `created` and `updated` |
| 3 | Cross-repo relationships in YAML only. Fields: `related`, `repo`, `ref` |
| 4 | YAML `id` field is the canonical link anchor. Format: `[[ID]]` |
| 5 | Existing files retain current naming. New convention applies to all new documents from 2026-03-19 forward |

---

## 3. Filename Structure

```
[TYPE]-[SEQ]-[slug].md
```

### Components

**TYPE** -- three-letter code defining what the document *is*. See Section 5 for the full registry.

**SEQ** -- three-digit zero-padded sequence number. Increments per TYPE, not globally.

```
001, 002, 003 ...
```

**slug** -- lowercase, hyphenated, human-readable description. Non-authoritative. The slug may be updated without breaking anything. The `id` field is the stable identity.

### Examples

```
ADR-001-capability-layer-boundary-design.md
LOG-001-knowledgehub-strategic-pivot-2026-03-19.md
TPL-001-naming-convention-system.md
INS-001-installation-first-run.ipynb
LAB-001-mistralai-py314-workaround.ipynb
```

---

## 4. YAML `id` Field

The `id` field is the canonical identity of every document. It is the anchor for all internal links.

### Format

```
[TYPE]-[SEQ]
```

### Examples

```
id: ADR-001
id: LOG-001
id: TPL-001
```

### Linking

Internal links from any document in any environment:

```
[[ADR-001]]
[[LOG-001]]
```

Links resolve against the `id` field, not the filename. Slug changes do not break links.

---

## 5. TYPE Code Registry

New TYPE codes may only be introduced via an ADR. No silent expansion.

### Architecture and Governance

| Code | Meaning |
|---|---|
| `ADR` | Architecture Decision Record |
| `GOV` | Governance policy or rule |
| `INT` | Intent Freeze |
| `INV` | Invariant definition |

### Documentation and Knowledge

| Code | Meaning |
|---|---|
| `DOC` | Reference document or overview |
| `SPC` | Specification |
| `SCH` | Schema definition |
| `GLO` | Glossary |

### Project and Session Management

| Code | Meaning |
|---|---|
| `SNP` | Snapshot -- state capture |
| `LOG` | Session log |
| `PLN` | Plan or workflow map |
| `GTE` | Gate or control checkpoint |

### Testing and Lab

| Code | Meaning |
|---|---|
| `INS` | Installation or first-run test |
| `LAB` | Lab notebook -- investigation |
| `TST` | Test document |
| `RUN` | Run log or execution record |

### Data and Reference

| Code | Meaning |
|---|---|
| `DAT` | Raw data or reference material |
| `IDX` | Index or registry |
| `TPL` | Template |

---

## 6. YAML Header Template

Every document. No exceptions.

```yaml
---
id: TYPE-001
title: Human readable title
type: type-code-lowercase
status: draft
version: "1.0"
created: YYYY-MM-DD
updated: YYYY-MM-DD
provenance: human
scope: []
tags: []
related: []
ref: []
repo: []
---
```

### Field Definitions

| Field | Required | Description |
|---|---|---|
| `id` | Yes | Canonical identity. Never changes. |
| `title` | Yes | Human-readable title. |
| `type` | Yes | TYPE code in lowercase. |
| `status` | Yes | Lifecycle status. See below. |
| `version` | Yes | Semantic version string. |
| `created` | Yes | ISO date of creation. |
| `updated` | Yes | ISO date of last update. |
| `tags` | No | List of relevant keywords. |
| `related` | No | IDs of related documents in same repo. |
| `ref` | No | IDs of referenced documents or findings. |
| `repo` | No | External repo references. Populated only when explicitly cross-referencing another repository. |
|    scope    |  Yes  |                                                Knowledgehub, governance, global                                                |

### Status Lifecycle

```
draft > active > locked > archived
```

| Status | Meaning |
|---|---|
| `draft` | Being written. Not yet authoritative. |
| `active` | Authoritative. In effect. |
| `locked` | Stable. Changes require a new superseding document. |
| `archived` | Obsolete or superseded. Retained for traceability. |

---

## 7. Version Control

Versions follow semantic notation: `MAJOR.MINOR`

- `MAJOR` increments on structural or authoritative changes
- `MINOR` increments on corrections or clarifications

Version is a string in YAML:

```yaml
version: "1.0"
version: "1.1"
version: "2.0"
```

---

## 8. Superseding a Locked Document

Locked documents are never edited. To supersede:

1. Create a new document with a new SEQ number
2. Add `related: [OLD-ID]` to the new document
3. Update the old document `status` to `archived`
4. Add a supersession notice at the top of the old document:

```markdown
> *Superseded by [[NEW-ID]] on YYYY-MM-DD.*
```

---

## 9. Transition Rule

This convention applies to all new documents from 2026-03-19 forward.

Existing documents across all repos retain their current naming and are not retroactively migrated. Where existing documents are referenced in new documents, use the existing ID or filename as the `related` or `ref` value.

---

*End of TPL-001*
