---
id: SNP-CUR-01
type: snp
status: active
version: "1.4"
created: 2026-02-13
updated: 2026-03-22
provenance: ai-assisted
scope: [knowledgehub]
tags: [snapshot, current-state, phase-5]
related: [LOG-003, LOG-004, LOG-005, ADR-003, ADR-004, ADR-005, ADR-006, ADR-007, ADR-008, ADR-009, TPL-001]
ref: []
repo: []
---

# CURRENT STATE

Control Pack Version: 2.0
Last Structural Change: 2026-03-22
Snapshot Version: 1.4

Phase 5 Status: ACTIVE — Content population in progress
Start Date: 2026-03-19
Governance Integrity: Verified
Structural Drift: None detected
Next Phase: N/A -- content population continues

Active File Under Revision: None

---

## SESSION RESUME PROTOCOL

Before executing any task, the assistant must:

1. Read `MASTER_PROMPT.md` in full.
2. Read `snapshots/SNP-CUR-01-current-state.md` in full.
3. Read `SESSION_PROMPT.md` in full.
4. Confirm alignment with all frozen rules and constraints.
5. Identify whether a new file is explicitly declared for revision.
6. State understanding of current priorities before acting.

No assumptions.
No reinterpretation.
No structural changes without explicit confirmation.

---

## 1. Project Status

Project: cjk-knowledgehub-governance
Purpose: Governance and control layer for the CJK KnowledgeHub rebuild

Current Phase:
Phase 5 active. Full visual design locked. IA skeleton locked. Governance
ADRs filed. mkdocs.yml and custom.css implemented. Bilingual support
(EN/DE) live via mkdocs-static-i18n. Site rendering locally. Content
population is the active work. Home and Projects sections complete.
Experience and Method sections partially complete (see below).

---

## 2. Completed

### Phase 1--4 (pre 2026-03-19)
- Repository scaffold created.
- Governance folder structured.
- Deterministic naming convention frozen.
- YAML schema v0.2 frozen.
- Folder hierarchy frozen.
- Deprecation protocol frozen.
- All legacy planning and snapshot files deprecated and archived.
- Phase 4 stabilisation complete.

### Phase 5 Initialisation (2026-03-19)
- Full strategic reset confirmed.
- Positioning pivoted to AI Systems Architecture.
- New IA confirmed: seven sections, artefact-first.
- INT-006 drafted and filed.
- LOG-001 filed. TPL-001 filed. MASTER_PROMPT v2.0 filed.
- DEPRECIATION_LOG updated.

### Phase 5 Pre-Build Locks (2026-03-19)
- Navigation order locked: Home · Projects · Experience · Method ·
  Credentials · About · Legacy.
- Simpleshow description locked per KH-004.
- Reference session: [[LOG-001]].

### Phase 5 Collaboration Setup (2026-03-20)
- Claude Project Files confirmed as static snapshots.
- Notion Collaboration Hub established as shared external memory.
- Dual-repo authority structure confirmed.
- LOG-002 filed.

### Phase 5 Visual Design, IA, and Build Foundation (2026-03-20, Session 6)
- VIS-004b locked: Cooper Hewitt / Barlow / Hack.
- `scope` field added to YAML schema via ADR-003.
- Navigation order locked: KH-012.
- IA skeleton locked: KH-013.
- Credentials page structure locked: KH-014.
- Contact approach locked: CON-001.
- Social footer locked: CON-002.
- ADR-003 through ADR-008 filed.
- mkdocs.yml and custom.css implemented and pushed.
- Site confirmed rendering locally. LOG-003 filed.

### Phase 5 Bilingual Build and Projects Content (2026-03-22, Sessions 7--8)
- Full bilingual support locked: KH-015. Plugin: mkdocs-static-i18n
  v1.3.1. German file convention: `.de.md` suffix.
- ADR-009 filed.
- Agentic Applications removed from nav and IA: KH-016.
- IO-III Architecture public name locked as 10³ Architecture: KH-017.
- Standing rule locked: no negative comparisons in copy; no punchy
  taglines outside CJK register.
- Content committed:
  - `docs/index.md` / `.de.md` -- v1.0, frozen
  - `docs/projects/index.md` / `.de.md` -- v0.1
  - `docs/projects/io-iii-architecture.md` / `.de.md` -- v0.2
  - `docs/projects/prompt-pattern-library.md` / `.de.md` -- v0.3
  - `docs/projects/knowledgehub-governance.md` / `.de.md` -- v0.1
- LOG-004 filed.

### Phase 5 Experience and Method Content (2026-03-22, Session 9)
- Experience section committed as single page EN and DE.
  - Client framing locked: "global clients in the banking, pharmacology,
    automotive, and tech industries."
  - Job title locked: "Conceptor & Project Manager."
  - Years of practice: 26 throughout.
- Method section: three pages committed EN and DE.
  - How I Work: working principles, ADR-first, constraints as features,
    drift anticipation.
  - Architecture Decision Records: practice explanation, links to
    io-architecture ADR index and KnowledgeHub governance repo.
  - Tools and Environment: comprehensive -- 15 categories covering AI/LLM
    infrastructure, LLM platforms, development, languages, statistical
    tools, knowledge/documentation, web/CMS, UI/UX, operating environment,
    admin/productivity, video/broadcast, audio, visual design/print,
    physical production skills, and teaching/lecturing.
- Content committed:
  - `docs/experience/index.md` / `.de.md` -- v0.1
  - `docs/method/how-i-work.md` / `.de.md` -- v0.2
  - `docs/method/architecture-decision-records.md` / `.de.md` -- v0.2
  - `docs/method/tools-and-environment.md` / `.de.md` -- v0.3
- LOG-005 filed.

---

## 3. In Progress / Held

| File | Status | Note |
|---|---|---|
| `docs/method/index.md` / `.de.md` | Held -- not committed | Content direction unresolved. Interdisciplinary Design Philosophy angle identified as correct framing. Opening domain list and "The material changes. The method holds." are strong. Third paragraph and close need rethinking. Begin next session here. |

---

## 4. Pending -- Content Population

Remaining sections to write:

1. Method index -- EN and DE (held, see above)
2. Credentials -- 25 certifications, two domains
3. About -- profile statement, contact
4. Legacy -- 26-year practice overview, artefacts

---

## 5. Next Immediate Task

Resolve Method index content direction. Produce and commit EN and DE.
Then proceed to Credentials section.

---

## 6. Visual Punch-List (Deferred to Polish Pass)

- Cooper Hewitt in nav reads slightly condensed at screen resolution.
  Fix: increase letter-spacing in custom.css during polish pass.

---

## 7. Standing Open Items

| Item | Carried from |
|---|---|
| TPL-001: `scope` field undocumented at v2.0 | Session 6 |
| German ß convention: "einschließlich" vs "einschliesslich" -- CJK to confirm preferred convention | Session 9 |

---

## Next Session Anchor

INT-006 is the current authoritative freeze.
Session log references: [[LOG-001]] [[LOG-002]] [[LOG-003]] [[LOG-004]] [[LOG-005]]
Governance ADRs: [[ADR-003]] through [[ADR-009]]
Naming convention: [[TPL-001]]
Master prompt: MASTER_PROMPT.md v2.0
Collaboration Hub: https://www.notion.so/329d296c3350814cbfa8cccac299d283

Status: Content population active. Method index held. Credentials next.

---

*This document must be updated whenever structural or authority changes occur.*