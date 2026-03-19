---
id: INT-006
title: KnowledgeHub Strategic Reset — Intent Freeze
type: int
status: locked
version: "1.1"
created: 2026-03-19
updated: 2026-03-19
provenance: ai-assisted
tags: [knowledgehub, intent-freeze, ia, positioning, reset]
related: [SNP-LOG-001, TPL-001]
ref: []
repo: []
---

# KnowledgeHub Strategic Reset — Intent Freeze

---

**Supersedes:** GOV-INT-02, GOV-INT-03, GOV-INT-04, GOV-INT-05
**Depends on:** GOV-INT-01 (Phase 1 Intent Freeze -- remains in force where not contradicted below)
**Status:** Locked

---

## 1. Purpose

This document freezes the strategic intent, positioning, and information architecture of the CJK KnowledgeHub following a full strategic reset on 2026-03-19.

It supersedes all prior architectural and execution intent freezes (GOV-INT-02 through GOV-INT-05). Those documents are to be deprecated per the governance deprecation protocol.

GOV-INT-01 (Phase 1 Intent Freeze) remains partially in force. Where GOV-INT-01 conflicts with this document, this document takes precedence.

No implementation, scaffolding, or content creation may begin until this freeze is confirmed by CJK.

---

## 2. Strategic Context

The KnowledgeHub was originally architected around prompt engineering as a primary positioning anchor. That framing is now obsolete. Prompt engineering has become a baseline skill across the industry, not a differentiating role.

The pivot is not a departure from what has been built. It is a correct reframing of what was always true: the work -- IO-III Architecture, the governance methodology, the testing and documentation standards -- has always been systems architecture work. The portfolio must now reflect that accurately.

---

## 3. Positioning

### Primary Positioning

**AI Systems Architecture**

The KnowledgeHub positions CJK as an AI systems architect: a practitioner who designs constraint-first systems, documents architectural decisions before implementing them, and applies structural discipline across technical and creative domains.

### Positioning Rules

- The site does not state "I am an AI systems architect." The structure and evidence make the argument.
- Prompt engineering is a skill present in the evidence layer. It is not a positioning anchor anywhere on the site.
- The 26-year professional history is not legacy baggage. It is the foundation of the working method. It is presented as such.
- The site is honest about the transition. It does not overstate current capability or understate demonstrated architectural thinking.

### Headline

Unchanged from current frozen state:

```
AI Systems Design | Governed LLM Infrastructure | Workflow Architecture
```

---

## 4. Core Argument

Every section of the KnowledgeHub must serve one argument:

*This is a person who designs systems with structural discipline, documents decisions before implementing them, and has been doing that in some form for 26 years.*

No section exists that does not contribute to this argument.

---

## 5. Audience

The KnowledgeHub serves a layered audience. Information architecture must reward each layer without penalising the others.

| Audience | Need |
|---|---|
| Recruiters and hiring managers | Clear positioning, evidence of value, legible history |
| Senior managers and directors | Strategic overview, judgement signals |
| Technical specialists | Depth, rigour, architectural decisions |
| Collaborators and peers | Method, working style, intellectual character |

CJK does not write down to any audience. All writing bridges intelligently.

---

## 6. Information Architecture

### Model

**Artefact-first.** The site leads with evidence, not biography.

### Top-Level Sections

Six sections confirmed. Navigation order to be locked in the next ADR.

---

#### Home

The landing page. A positioning statement, not a CV. Short, authoritative, links inward to evidence.

---

#### Work

The primary evidence layer. Three subsections:

**Projects**
Full case study treatment for each project. Not README reprints. Human-readable accounts of architectural thinking, decisions made, and method demonstrated.

Confirmed projects:
- IO-III Architecture -- flagship. Six-phase governed LLM control-plane runtime. ADR-first methodology. Phases 1--3 complete and hardened. Phase 4 active.
- Prompt Pattern Library -- paused but architecturally complete. 19-domain taxonomy, YAML and Markdown schema, MkDocs publication architecture. Status stated honestly.
- cjk-knowledgehub-governance -- governance architecture applied to a real system. Demonstrates ADR methodology, deterministic naming, layered authority hierarchy, and deprecation protocol. A working artefact of the same discipline as IO-III.
- Agentic-Applications fork (manuasdf/Agentic-Applications, branch cjk-glitch-ministry) -- demonstrates structured testing methodology, reproducible documentation, bug diagnosis, and merged OSS contribution.

**Professional History**
A continuous working biography, not a CV list. Three entries:
- Simpleshow GmbH -- Conceptor and Project Manager, Nov 2020--Dec 2024. Canonical description: DAT-CV-CJK-001-en-2026-03-10.md. Exact wording correction from CJK pending.
- Independent Practice -- Interdisciplinary Media Designer, May 1999--Jun 2025.
- LUDWIG Bar / Gallery / Venue -- Co-owner and Operator, Dec 2015--Sep 2019.

**Contributions**
OSS contributions and external work. Opens with the Agentic-Applications PR. Grows over time.

---

#### Method

The architectural thinking layer. Differentiates CJK from candidates who list tools.

Three subsections:
- *Architecture Decision Records* -- IO-III ADRs surfaced and explained for a general technical audience.
- *Design Principles* -- Constraint-first design, explicit decisions, boundaries before building. The intellectual position stated plainly.
- *Testing and Documentation Standards* -- The INS/LAB methodology. Reproducibility as a practice, not an afterthought.

---

#### Credentials

25 certifications presented as a coherent progression narrative. Not a badge wall.

Canonical source: Bildungsgutschein Anlage 6 (25 entries, verified 2026-02-18).

Three clusters:
- AI Engineering and Governance
- Statistical and Mathematical Foundations
- Python and Development Tooling

---

#### About

Single page. First person. The arc from 1999 to now. Honest about the transition. Headshot lives here.

---

#### Creative

A dedicated section honouring CJK's creative history with its own artefacts. Presented on its own terms, not subordinated to the AI work. The right audience reads it correctly.

Scope, content, and structure to be defined in a future ADR. Not current build priority.

---

## 7. Site Principles

### Full Replacement

The existing site is a complete replacement, not an incremental overhaul. The existing mkdocs.yml and content structure are deprecated.

### The Site Is an Artefact

The KnowledgeHub is not merely a presentation layer. It is itself a portfolio artefact. Its architecture, methodology, and execution demonstrate the same systems thinking it describes. The cjk-knowledgehub-governance repo is a parallel workstream and itself a demonstration of governance discipline.

### All Repos Are Artefacts

Every repository in CJK's ecosystem is intentionally layered. Each is both a working system and a demonstration of method. This principle applies to IO-III, the Prompt Pattern Library, the KnowledgeHub, the Agentic-Applications fork, and the governance repo.

### No Constraints on Audience Intelligence

CJK does not simplify content for a lower common denominator. All writing bridges intelligently -- respecting the reader's intelligence and demonstrating CJK's own.

---

## 8. Supersession and Deprecation

The following documents are superseded by this freeze and must be formally deprecated per the governance deprecation protocol:

| Document | Reason |
|---|---|
| GOV-INT-02 | IA obsolete; Vective substrate removed; new domains locked |
| GOV-INT-03 | Execution plan built on obsolete IA |
| GOV-INT-04 | Repository structure built on obsolete IA |
| GOV-INT-05 | Vective evaluation doctrine -- Vective deprecated entirely |
| mkdocs.yml (current) | Reflects old six-domain structure |

Deprecation procedure per MASTER_PROJECT_PROMPT.md Section 7.

---

## 9. Open Items

The following items are not yet locked and must be resolved before build begins:

| Item | Owner | Priority |
|---|---|---|
| Simpleshow description exact wording | CJK | High |
| Navigation order for six sections | CJK + Claude | High |
| Creative section scope and content | CJK | Low -- deferred to ADR |

---

## 10. Locked Decisions Reference

All KH and NC decisions locked in session SNP-LOG-001 are in force. See [[SNP-LOG-001]] for the full decision log.

---

## 11. Freeze Conditions

This document is locked and authoritative from 2026-03-19.

It may only be superseded by a new INT document explicitly referencing this one.

No implementation, scaffolding, or content creation for the KnowledgeHub rebuild may begin without CJK's explicit confirmation that this freeze is accepted.

---

*End of INT-006 v1.1*
