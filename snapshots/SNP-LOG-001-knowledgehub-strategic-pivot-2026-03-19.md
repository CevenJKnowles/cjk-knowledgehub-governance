---
id: SNP-LOG-001
title: KnowledgeHub Strategic Pivot
type: log
status: active
version: "1.1"
created: 2026-03-19
updated: 2026-03-19
tags: [knowledgehub, strategy, ia, pivot, naming-convention]
related: [TPL-001]
ref: []
repo: []
---

# Session Log — KnowledgeHub Strategic Pivot

---

**Date:** 2026-03-19
**Session type:** Strategy and IA reset
**Conducted via:** Claude Sonnet 4.6 / claude.ai

---

## 1. Context

The KnowledgeHub has sat dormant since Phase 4 locked in February 2026. Significant changes in strategic direction, personal priorities, and market understanding have made the existing Phase 2 Architecture Freeze obsolete. This session constitutes a full strategic reset, confirming a new positioning, a new information architecture, and a new trajectory for Phase 5.

This document records all decisions locked in this session. It is the authoritative source for the new Intent Freeze, which must be drafted as a formal INT document superseding GOV-INT-02.

---

## 2. Supersession Notice

The following documents are superseded by this session. Formal deprecation via GOV procedure is pending.

| Document | Status | Reason |
|---|---|---|
| GOV-INT-02 (Phase 2 Architecture Freeze) | To be deprecated | IA obsolete; Vective substrate removed; new domains locked |
| mkdocs.yml (current) | To be deprecated | Reflects old six-domain structure |
| Phase 5 definition in PLN-MAP-01 | To be superseded | "Prompt Engineering Artifact Construction" is no longer the correct Phase 5 objective |

No files deleted. Deprecation protocol applies.

---

## 3. Locked Decisions

All decisions below are authoritative from this session forward.

### KnowledgeHub Positioning and Structure

| ID | Decision |
|---|---|
| KH-001 | Positioning: AI Systems Architecture. Existing headline unchanged. Evidence layer to be rebuilt to reflect this. |
| KH-002 | Prompt engineering is a skill, not a role. Not a positioning anchor anywhere on the site. |
| KH-003 | Bildungsgutschein: out of scope for KnowledgeHub entirely. |
| KH-004 | Simpleshow description: CV version (DAT-CV-CJK-001-en-2026-03-10.md) is canonical. Exact wording correction from CJK pending. |
| KH-005 | Certifications: Bildungsgutschein Anlage 6 is the authoritative source. 25 total. |
| KH-006 | Full replacement of existing site. Clean slate IA. Not incremental overhaul. |
| KH-007 | All repos are intentionally layered artefacts. cjk-knowledgehub-governance is in scope as a parallel workstream. The KnowledgeHub is itself a portfolio artefact, not merely a presentation layer. |
| KH-008 | Agentic-Applications fork (manuasdf/Agentic-Applications, branch cjk-glitch-ministry) is a confirmed portfolio artefact. Includes INS-001, LAB-001, manu-aa-test-1.md, SESSION-2026-03-17. Demonstrates: structured testing methodology, reproducible documentation, bug diagnosis and fix, merged OSS PR. |
| KH-009 | A dedicated Creative section is confirmed for the KnowledgeHub. Scope, content, and structure to be defined in a future ADR. Not current priority. |

### Naming Convention System

| # | Decision |
|---|---|
| NC-001 | No repo identifier in filename. |
| NC-002 | Date in YAML only. Fields: `created` and `updated`. |
| NC-003 | Cross-repo relationships in YAML only. Fields: `related`, `repo`, `ref`. |
| NC-004 | YAML `id` field is the canonical link anchor. Format: `[[ID]]`. |
| NC-005 | Existing files retain current naming. New convention applies to all new documents from 2026-03-19 forward. No retroactive migration. |

Full convention documented in [[TPL-001]].

---

## 4. New Information Architecture

Six top-level sections confirmed. Navigation order is indicative only -- to be locked in the new Intent Freeze.

---

### Home

Positioning statement. Not a CV. Short, authoritative, links inward.

---

### Work

Three subsections:

*Projects* -- IO-III Architecture, Prompt Pattern Library, Agentic-Applications fork. Full case study treatment per project.

*Professional History* -- Simpleshow, Independent Practice, LUDWIG. Continuous working biography, not a CV list.

*Contributions* -- OSS contributions and external work. Opens with Agentic-Applications PR.

---

### Method

*Architecture Decision Records* -- IO-III ADRs surfaced for a general technical audience.

*Design Principles* -- Constraint-first design, explicit decisions, boundaries before building.

*Testing and Documentation Standards* -- INS/LAB methodology. Reproducibility as practice.

---

### Credentials

Certifications and learning trajectory presented as a coherent progression narrative. Not a badge wall.

---

### About

Single page. First person. The arc from 1999 to now. Headshot lives here.

---

### Creative

Dedicated section honouring creative history with its own artefacts. Scope to be defined in a future ADR. Not current build priority.

---

## 5. Core Positioning Statement

The KnowledgeHub does not claim "I am an AI systems architect." The structure and evidence make the argument without stating it.

**The argument the site must make:** This is a person who designs systems with structural discipline, documents decisions before implementing them, and has been doing that in some form for 26 years.

---

## 6. Source of Truth Hierarchy

1. This document ([[SNP-LOG-001]])
2. Project files in cjk-knowledgehub-governance repo
3. DAT-CV-CJK-001-en-2026-03-10.md (canonical CV -- English)
4. Bildungsgutschein Anlage 6 (canonical certification list, 25 entries)

---

## 7. Immediate Next Actions

| Priority | Action |
|---|---|
| 1 | Update SNP-CUR-01 in governance repo to point to this document as session anchor |
| 2 | File TPL-001 in governance repo |
| 3 | Draft new Intent Freeze (INT-003) superseding GOV-INT-02 |
| 4 | Deprecate GOV-INT-02 per protocol |
| 5 | Draft new Phase 5 definition superseding PLN-MAP-01 entry |
| 6 | Draft ADR for Creative section scope |
| 7 | Begin new mkdocs.yml scaffold aligned to new IA |

---

## 8. Open Items

- **Simpleshow description:** exact correction not yet provided. CJK to confirm precise wording before any draft references it.
- **Navigation order:** six sections confirmed, order indicative only. To be locked in INT-003.
- **Creative section scope:** deferred to ADR.

---

*End of SNP-LOG-001 v1.1*
