---
id: SNP-CUR-01
title: Current State Snapshot
type: snp
status: active
version: "2.0"
created: 2026-02-13
updated: 2026-04-13
provenance: ai-assisted
scope: knowledgehub
tags: [snapshot, current-state, phase-5]
related: [LOG-003, LOG-004, LOG-005, LOG-006, LOG-007, ADR-003, ADR-004, ADR-005, ADR-006, ADR-007, ADR-008, ADR-009, ADR-010, ADR-011, ADR-012, TPL-001]
ref: []
repo: []
---

# CURRENT STATE

Control Pack Version: 2.0
Last Structural Change: 2026-04-13
Snapshot Version: 2.0

Phase 5 Status: ACTIVE — Content complete. Visual polish complete. Pre-launch.
Start Date: 2026-03-19
Governance Integrity: Verified
Structural Drift: None detected
Next Phase: Phase 6 — Domain redirect and public launch

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
Phase 5 complete. All seven content sections committed in EN and DE.
Visual polish pass executed. Font switched to Lexend Exa (ADR-012).
Sidebar social widget implemented. Site is in a publishable state.
Phase 6 (domain redirect and public launch) is next.

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
- Home page revised to align with KH-018 arc. v2.0 committed.
- Credentials section produced: 25 certs linked to hosted JPGs.
- Three directory issues resolved.
- Content committed:
  - `docs/method/index.md` / `.de.md` -- v0.1
  - `docs/index.md` / `.de.md` -- v2.0
  - `docs/credentials/index.md` / `.de.md` -- v0.1
- LOG-006 filed.

### Phase 5 About, Legacy, Visual Polish, Font Switch (2026-04-13, Session 11)
- ß convention locked: ß over SS throughout all German files.
- TPL-001 v2.0 committed: `scope` field formally documented.
- ADR-012 filed: Lexend Exa replaces Cooper Hewitt (supersedes VIS-004b).
- About section produced EN and DE. First-person, warm register.
- Legacy section produced EN and DE. Chronological essay with links.
  Covers Anderecast, Cerusmedia, Lesley Rankine/Ruby, The Opiates,
  Hinausgehen, ELECTROSEXUAL Best Music Video 2021, LUDWIG 2016--2019,
  CHAOSTROPHY, public record.
- Visual polish pass:
  - pymdownx.emoji extension added (fixes icon rendering)
  - Social icons switched to Simple Icons prefix throughout
  - YouTube and Substack added to social list
  - Sidebar social widget implemented via overrides/partials/nav.html
  - Contact email as plain selectable text (anti-spam)
  - Nav tab colours: light inactive #efefef / active #ff6700;
    dark inactive #ff6700 / active #efefef
  - UI icons (language, day/night): #ff6700 both modes
  - Repo link visibility fixed for light mode
  - Logo size set to 2.5rem
- Content committed:
  - `docs/about/index.md` / `.de.md` -- v0.3 / v0.1
  - `docs/legacy/index.md` / `.de.md` -- v0.5 / v0.1
- LOG-007 filed.

---

## 3. In Progress / Held

None.

---

## 4. Pending — Pre-Launch

1. Cooper Hewitt font files cleanup commit
   Remove `docs/assets/fonts/cooperhewitt/` once final visual review confirmed
2. Stack Overflow profile URL verification before publish
3. Contact form — Formspree implementation deferred; email displayed as
   plain text in sidebar widget for now
4. Final visual review on live/staging environment

---

## 5. Next Immediate Task

Phase 6: Domain redirect cevenknowles.com → GitHub Pages.

---

## 6. Visual Punch-List

- Cooper Hewitt cleanup commit pending
- Stack Overflow URL to verify

---

## 7. Standing Open Items

| Item | Status |
|---|---|
| Cooper Hewitt files removal | Pending cleanup commit |
| Stack Overflow URL | Needs verification |
| Contact form (Formspree) | Deferred — plain text email in sidebar for now |

---

## Next Session Anchor

INT-006 is the current authoritative freeze.
KH-018 (ADR-011) is the canonical narrative invariant.
Session log references: [[LOG-001]] through [[LOG-007]]
Governance ADRs: [[ADR-003]] through [[ADR-012]]
Naming convention: [[TPL-001]] v2.0
Master prompt: MASTER_PROMPT.md v2.0
Collaboration Hub: https://www.notion.so/329d296c3350814cbfa8cccac299d283

Status: All content complete. Visual polish complete. Pre-launch.

---

*This document must be updated whenever structural or authority changes occur.*
