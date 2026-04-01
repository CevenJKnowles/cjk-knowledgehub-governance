---
id: LOG-006
title: "LOG | Session 10 — Scope Realignment, Method Index, Home, Credentials — 2026-04-01"
type: log
status: active
version: "1.0"
created: 2026-04-01
updated: 2026-04-01
provenance: ai-assisted
scope: [knowledgehub]
tags: [session-log, phase-5, content, method, credentials, home, scope, adr]
related: [LOG-005, ADR-010, ADR-011, SNP-CUR-01]
ref: []
repo: []
---

# LOG | Session 10 — Scope Realignment, Method Index, Home, Credentials — 2026-04-01

---

## Session Summary

Four workstreams completed: Method index content production, strategic scope
realignment, Home page revision, and Credentials section production.

---

## 1. Method Index — Content Resolved and Committed

The Method index content direction was unresolved at the close of Session 9.
The Interdisciplinary Design Philosophy angle had been identified as correct
but not fully executed.

CJK submitted a revised text. Four of six paragraphs were assessed as working.
Two required revision: Para 2 was too generic and missed the cross-domain
distinctiveness; Para 5 was still navigational. A revised version was produced
with the domain list leading Para 2 and Para 5 rewritten to describe three
levels of visibility without naming or signposting sub-pages.

CJK confirmed the text. Both files committed.

- `docs/method/index.md` -- v0.1, committed
- `docs/method/index.de.md` -- v0.1, committed

---

## 2. Copy Rule Locked — COP-001

During the Method index revision, the "26 years" / "26-year" pattern was
identified as overused across the site. CJK confirmed it should stop.

Decision locked: no tenure figures in body copy anywhere on the site, in
either language. The domain list carries the weight of breadth. This does
not apply to the GitHub profile, LinkedIn, or CV, where format convention
may make a tenure figure appropriate.

Governance ID: COP-001. Filed as ADR-010.

---

## 3. Scope Realignment — Canonical Narrative Invariant Locked

CJK raised a strategic observation: the job market at his actual experience
level is better served by a coherent generalist systems narrative than by
framing that reaches toward positions requiring qualifications not yet held.

CJK proposed and confirmed the Canonical Narrative Invariant document,
establishing a single governing question for all site content:

What allows a complex thing to hold together as conditions change?

The document includes the core thesis, primary scope goal, section-level
alignment contracts for all seven nav items, a Global Writing Rule (per-page
testable challenge), and an editorial QA checklist.

One conflict was flagged and resolved before locking: the About section scope
sentence used "a 26-year practice", conflicting with COP-001. Corrected to
"a sustained interdisciplinary practice" before lock.

Governance ID: KH-018. Filed to Notion Collaboration Hub and as ADR-011.

---

## 4. Home Page — Revised and Committed

The Home page was revised to align with the Home to Projects to Method arc
established by KH-018. Para 3 (method steps) was identified as duplicating
Method and cut. A single bridge sentence ("The method is consistent. The
context it now operates in is not.") replaced it. Para 4 (current AI context)
was expanded from two sentences to a full paragraph. The signage paragraph
(Para 5) was removed entirely.

This unfreezes `docs/index.md` from v1.0 (frozen Session 7). CJK confirmed
the unfreeze was intentional.

- `docs/index.md` -- v2.0, committed (replaces frozen v1.0)
- `docs/index.de.md` -- v2.0, committed (replaces frozen v1.0)

---

## 5. Credentials — Produced and Committed

Credentials section produced with domain-level interpretation agreed by CJK.
Each domain receives a lead-in paragraph interpreting the learning through
the structural method, followed by a scannable list with each certificate name
linked to its hosted JPG in `docs/assets/certificates/`.

Three directory issues were also resolved before committing:
- `docs/method/index-de.md` renamed to `docs/method/index.de.md` (hyphen
  instead of dot would have broken mkdocs-static-i18n language switching).
- Three stray files removed from `docs/credentials/`: `credentials.md`,
  `ai-engineering-governance.md`, `statistical-mathematical.md`.
- `docs/projects/agentic-applications.md` deleted per KH-016 (out of scope).

- `docs/credentials/index.md` -- v0.1, committed
- `docs/credentials/index.de.md` -- v0.1, committed

---

## 6. Files Committed This Session

| File | Version | Status |
|---|---|---|
| `docs/method/index.md` | v0.1 | Committed |
| `docs/method/index.de.md` | v0.1 | Committed |
| `docs/index.md` | v2.0 | Committed (unfrozen) |
| `docs/index.de.md` | v2.0 | Committed (unfrozen) |
| `docs/credentials/index.md` | v0.1 | Committed |
| `docs/credentials/index.de.md` | v0.1 | Committed |

---

## 7. Open Items Carried Forward

| Item | Carried from |
|---|---|
| TPL-001: `scope` field undocumented at v2.0 | Session 6 |
| German ß convention: `einschließlich` vs `einschliesslich` | Session 9 |
| Cooper Hewitt nav letter-spacing | Session 6 |

---

## 8. Agreed Next Steps

1. About section EN and DE
2. Legacy section EN and DE
3. Visual polish pass on custom.css once all content is in place

---

*Session 10 closed: 2026-04-01 CET*
