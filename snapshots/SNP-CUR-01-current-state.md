---
id: SNP-CUR-01
type: snp
status: active
version: "1.3"
created: 2026-02-13
updated: 2026-03-20
provenance: ai-assisted
scope: [knowledgehub]
tags: [snapshot, current-state, phase-5]
related: [LOG-003, ADR-003, ADR-004, ADR-005, ADR-006, ADR-007, ADR-008, TPL-001]
ref: []
repo: []
---

# CURRENT STATE

Control Pack Version: 2.0
Last Structural Change: 2026-03-20
Snapshot Version: 1.3

Phase 5 Status: ACTIVE — Build in progress
Start Date: 2026-03-19
Governance Integrity: Verified
Structural Drift: None detected
Next Phase: N/A -- content population

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
Phase 5 active. Full visual design locked. IA skeleton locked. Governance ADRs
filed. mkdocs.yml and custom.css implemented. Site rendering locally. Content
population is the next work.

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
- New IA confirmed: six sections, artefact-first.
- INT-006 drafted and filed -- supersedes GOV-INT-02 through GOV-INT-05.
- GOV-INT-02 through GOV-INT-05 archived.
- LOG-001 filed.
- TPL-001 (unified naming convention) filed.
- MASTER_PROMPT v2.0 filed -- supersedes DEP-MASTER_PROJECT_PROMPT_v1.md.
- DEPRECIATION_LOG updated.
- Governance repo committed and pushed.

### Phase 5 Pre-Build Locks (2026-03-19, KnowledgeHub Reboot Meeting)
- Navigation order locked: Home · Work · Method · Credentials · About · Legacy.
- Sixth section renamed from "Creative" to "Legacy".
- Simpleshow description locked per KH-004.
- All pre-build blocking items from INT-006 Section 9 resolved.
- Reference session: [[LOG-001]].

### Phase 5 Collaboration Setup (2026-03-20)
- Claude Project Files confirmed as static snapshots. Manual re-upload workflow established.
- GitHub repos confirmed accessible to Claude via GitHub integration.
- Notion Collaboration Hub established as shared external memory.
- Dual-repo authority structure confirmed.
- INT-006 reviewed and confirmed as active authoritative freeze.
- LOG-002 filed.

### Phase 5 Visual Design, IA, and Build Foundation (2026-03-20, Session 6)
- VIS-004 voided (logged in error). VIS-004b locked: Cooper Hewitt / Barlow / Hack.
- `scope` field added to YAML schema via ADR-003.
- Navigation order updated: Home · Projects · Experience · Method · Credentials
  · About · Legacy. KH-010 superseded by KH-012.
- IA skeleton locked: KH-013. Seven sections fully defined.
- Credentials page structure locked: KH-014. 25 certifications, two domains.
- Contact approach locked: CON-001. hello@cevenknowles.com + Formspree.
- Social footer locked: CON-002. Six platforms confirmed.
- ADR-003 through ADR-008 filed to governance/.
- mkdocs.yml fully updated and pushed.
- custom.css created and pushed. Full visual design implementation.
- Cooper Hewitt font files self-hosted at docs/assets/fonts/cooperhewitt/.
- Docs structure updated to match locked nav. Old work/ directory removed.
- Site confirmed rendering locally via mkdocs serve. No errors.
- LOG-003 filed.
- SNP-CUR-01 updated (this document, v1.3).

---

## 3. In Progress

None.

---

## 4. Pending -- Content Population

Site is rendering. All structural and visual decisions are locked.
Content to be written for each section in order:

1. Home — hero statement, positioning, signpost cards
2. Projects — IO-III, Prompt Pattern Library, Governance repo, Agentic Applications
3. Experience — Simpleshow, IMD, LUDWIG
4. Method — How I Work, ADRs, Tools and Environment
5. Credentials — 25 certifications, two domains
6. About — profile statement, contact
7. Legacy — 26-year practice overview, artefacts

---

## 5. Next Immediate Task

Begin content planning and writing. Start with Home page.

---

## 6. Visual Punch-List (Deferred to Polish Pass)

- Cooper Hewitt in nav reads slightly condensed at screen resolution.
  Fix: increase letter-spacing in custom.css during polish pass.

---

## Next Session Anchor

INT-006 is the current authoritative freeze.
Session decisions (2026-03-19): [[LOG-001]]
Session decisions (2026-03-20 setup): [[LOG-002]]
Session decisions (2026-03-20 build): [[LOG-003]]
Governance ADRs: [[ADR-003]] [[ADR-004]] [[ADR-005]] [[ADR-006]] [[ADR-007]] [[ADR-008]]
Naming convention: [[TPL-001]]
Master prompt: MASTER_PROMPT.md v2.0
Collaboration Hub: https://www.notion.so/329d296c3350814cbfa8cccac299d283

Status: Site rendering. Content population is next.

---

*This document must be updated whenever structural or authority changes occur.*
