---
id: SNP-CUR-01
type: snp
status: active
version: "1.5"
created: 2026-02-13
updated: 2026-04-01
provenance: ai-assisted
scope: [knowledgehub]
tags: [snapshot, current-state, phase-5]
related: [LOG-003, LOG-004, LOG-005, LOG-006, ADR-003, ADR-004, ADR-005, ADR-006, ADR-007, ADR-008, ADR-009, ADR-010, ADR-011, TPL-001]
ref: []
repo: []
---

# CURRENT STATE

Control Pack Version: 2.0
Last Structural Change: 2026-04-01
Snapshot Version: 1.5

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
ADRs filed (ADR-003 through ADR-011). mkdocs.yml and custom.css implemented.
Bilingual support (EN/DE) live via mkdocs-static-i18n. Site rendering
locally. Content population is the active work. Home, Projects, Experience,
Method (all four pages), and Credentials are committed. About and Legacy
remain.

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
  - `docs/index.md` / `.de.md` -- v1.0, frozen (superseded Session 10)
  - `docs/projects/index.md` / `.de.md` -- v0.1
  - `docs/projects/io-iii-architecture.md` / `.de.md` -- v0.2
  - `docs/projects/prompt-pattern-library.md` / `.de.md` -- v0.3
  - `docs/projects/knowledgehub-governance.md` / `.de.md` -- v0.1
- LOG-004 filed.

### Phase 5 Experience and Method Content (2026-03-22, Session 9)
- Experience section committed as single page EN and DE.
- Method section: three pages committed EN and DE.
- Content committed:
  - `docs/experience/index.md` / `.de.md` -- v0.1
  - `docs/method/how-i-work.md` / `.de.md` -- v0.2
  - `docs/method/architecture-decision-records.md` / `.de.md` -- v0.2
  - `docs/method/tools-and-environment.md` / `.de.md` -- v0.3
- LOG-005 filed.

### Phase 5 Scope Realignment, Method Index, Home, Credentials (2026-04-01, Session 10)
- Method index content direction resolved. Text confirmed and committed.
- Copy rule locked: no tenure figures in body copy. COP-001. ADR-010 filed.
- Canonical Narrative Invariant locked: KH-018. ADR-011 filed.
  Core thesis: "What allows a complex thing to hold together as conditions
  change?" governs all content. Section-level contracts locked for all seven
  nav items. Global Writing Rule and editorial QA checklist locked.
- Home page revised to align with KH-018 arc. Para 3 cut (duplicated Method).
  Bridge sentence added. Para 4 expanded. Signage paragraph removed.
  Unfreezes v1.0 (frozen Session 7) with CJK confirmation.
- Credentials section produced: domain-level interpretation, 25 certs linked
  to hosted JPGs in `docs/assets/certificates/`.
- Three directory issues resolved: method index DE filename corrected,
  stray credentials files removed, agentic-applications.md deleted (KH-016).
- Content committed:
  - `docs/method/index.md` / `.de.md` -- v0.1
  - `docs/index.md` / `.de.md` -- v2.0 (replaces frozen v1.0)
  - `docs/credentials/index.md` / `.de.md` -- v0.1
- LOG-006 filed.

---

## 3. In Progress / Held

None.

---

## 4. Pending -- Content Population

Remaining sections to write:

1. About -- profile statement, obfuscated email, Formspree contact form
2. Legacy -- practice overview, artefacts, Behance and Instagram links

---

## 5. Next Immediate Task

About section EN and DE.

---

## 6. Visual Punch-List (Deferred to Polish Pass)

- Cooper Hewitt in nav reads slightly condensed at screen resolution.
  Fix: increase letter-spacing in custom.css during polish pass.

---

## 7. Standing Open Items

| Item | Carried from |
|---|---|
| TPL-001: `scope` field undocumented at v2.0 | Session 6 |
| German ß convention: "einschließlich" vs "einschliesslich" -- CJK to confirm | Session 9 |

---

## Next Session Anchor

INT-006 is the current authoritative freeze.
KH-018 (ADR-011) is the canonical narrative invariant. All pages must be
validated against the Global Writing Rule before commit.
Session log references: [[LOG-001]] [[LOG-002]] [[LOG-003]] [[LOG-004]] [[LOG-005]] [[LOG-006]]
Governance ADRs: [[ADR-003]] through [[ADR-011]]
Naming convention: [[TPL-001]]
Master prompt: MASTER_PROMPT.md v2.0
Collaboration Hub: https://www.notion.so/329d296c3350814cbfa8cccac299d283

Status: Content population active. About section next.

---

*This document must be updated whenever structural or authority changes occur.*
