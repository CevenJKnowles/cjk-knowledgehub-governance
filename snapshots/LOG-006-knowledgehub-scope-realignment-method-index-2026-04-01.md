---
id: LOG-006
title: "LOG | Session 10 — Scope Realignment and Method Index — 2026-04-01"
type: log
status: active
version: "1.0"
created: 2026-04-01
updated: 2026-04-01
provenance: ai-assisted
scope: [knowledgehub]
tags: [session-log, phase-5, content, method, scope, adr]
related: [LOG-005, ADR-010, ADR-011, SNP-CUR-01]
ref: []
repo: []
---

# LOG | Session 10 — Scope Realignment and Method Index — 2026-04-01

---

## Session Summary

Session began with an init from the Notion Collaboration Hub. Two primary
workstreams were completed: Method index content production and a strategic
scope realignment.

---

## 1. Method Index — Content Resolved and Delivered

The Method index content direction was unresolved at the close of Session 9.
The Interdisciplinary Design Philosophy angle had been identified as correct
but not fully executed.

In this session, CJK submitted a revised text for assessment. Four of six
paragraphs were assessed as working. Two required revision:

- Para 2 was too generic -- it described good professional practice without
  connecting the cross-domain distinctiveness that is the site's actual claim.
- Para 5 was still navigational -- naming sub-pages and describing their
  function rather than functioning as genuine prose.

A revised version was produced. The domain list (broadcasting, education,
print, systems design, AI infrastructure) replaced the "26-year" opening in
Para 2, resolving the COP-001 issue simultaneously. Para 5 was rewritten to
describe three levels of visibility without naming or signposting sub-pages.

CJK confirmed the revised text. Files produced and delivered:

- `docs/method/index.md` -- v0.1, confirmed, ready to commit
- `docs/method/index.de.md` -- v0.1, confirmed, ready to commit

Status: awaiting CJK commit. Not yet in the repo.

---

## 2. Copy Rule Locked — COP-001

During the Method index revision, the "26 years" / "26-year" pattern was
identified as overused across the site. CJK confirmed it should stop.

Decision locked: No tenure figures in body copy anywhere on the site, in
either language. The domain list carries the weight of breadth.

Governance ID: COP-001. Filed as ADR-010 in this session.

---

## 3. Scope Realignment — Canonical Narrative Invariant Locked

CJK raised a strategic observation: the job market for his actual experience
level is better served by a coherent generalist systems narrative than by
framing that reaches toward positions requiring qualifications not yet held.

CJK proposed and confirmed a Canonical Narrative Invariant document
establishing a single governing question for all site content:

What allows a complex thing to hold together as conditions change?

The document includes:
- Core thesis
- Primary scope goal
- Section-level alignment contracts for all seven nav items
- A Global Writing Rule (per-page testable challenge)
- An editorial QA checklist

One conflict was flagged and resolved before locking: the About section
scope sentence used "a 26-year practice", which conflicts with COP-001.
Corrected to "a sustained interdisciplinary practice" before lock.

Governance ID: KH-018. Filed to Notion Collaboration Hub and as ADR-011
in this session.

---

## 4. Files Committed This Session

None. Session was content production and governance. Commits pending.

---

## 5. Files Ready to Commit

| File | Version | Status |
|---|---|---|
| `docs/method/index.md` | v0.1 | Confirmed, awaiting commit |
| `docs/method/index.de.md` | v0.1 | Confirmed, awaiting commit |
| `governance/ADR-010-copy-rule-no-tenure-figures.md` | v1.0 | This session |
| `governance/ADR-011-scope-alignment-canonical-narrative-invariant.md` | v1.0 | This session |

---

## 6. Open Items Carried Forward

| Item | Carried from |
|---|---|
| TPL-001: `scope` field undocumented at v2.0 | Session 6 |
| German ß convention: `einschließlich` vs `einschliesslich` | Session 9 |
| Cooper Hewitt nav letter-spacing | Session 6 |

---

## 7. Agreed Next Steps

1. CJK commits Method index EN and DE to main repo.
2. CJK commits ADR-010 and ADR-011 to governance repo.
3. Move to Credentials section content production.
4. Visual polish pass on custom.css once all content is in place.

---

*Session 10 closed: 2026-04-01 CET*
