---
id: ADR-005
title: "ADR | Top-Level Navigation Order"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [information-architecture, navigation, ux]
related: [ADR-006]
ref: []
repo: []
---

# ADR | Top-Level Navigation Order

---

## Context

An earlier locked decision (KH-010, 2026-03-19) established the top-level navigation as:

`Home · Work · Method · Credentials · About · Legacy`

During IA planning in Session 6, two problems were identified:

1. "Work" conflates two fundamentally different categories: open-source portfolio artefacts (GitHub repos) and professional employment history. Mixing them under a single label dilutes both.
2. The label "Work" is accurate for employment history but misleading for independently designed and owned artefacts.

A 7-item navigation was also considered and initially rejected on wrap-risk grounds. Testing confirmed that MkDocs Material's hamburger breakpoint at 1220px eliminates the wrap risk entirely — the menu collapses to a drawer before the viewport is ever narrow enough to cause a two-row layout. This makes 7 items structurally safe.

---

## Decision

Top-level navigation order locked as:

**Home · Projects · Experience · Method · Credentials · About · Legacy**

Seven items. No dropdowns at top level. MkDocs Material hamburger behaviour handles mobile and small-screen collapse automatically.

---

## Alternatives Considered

**Keep "Work", disambiguate internally** — evaluated. Would avoid reopening KH-010. Rejected because the label mismatch is a genuine accuracy problem, not a cosmetic one. A recruiter scanning "Work" expects employment history, not open-source architecture projects.

**"Portfolio" as a single unified label** — evaluated. Covers both artefacts and employment history under a familiar creative-portfolio convention. Rejected because the target audience is technical — "Projects" and "Experience" are immediately understood as distinct categories by senior engineers and hiring managers.

**6-item nav with Legacy under About** — evaluated. Would have kept the nav tighter. Rejected after MkDocs Material breakpoint testing confirmed wrap risk is non-existent. Legacy earns standalone visibility given the 26-year scope of the content.

**5-item nav with About containing Bio, Credentials, Legacy** — evaluated. Clean and minimal. Rejected because Credentials is verified external validation of technical competence — burying it under "About" reduces its visibility to a technical audience where it is a primary proof point.

---

## Rationale

"Projects" and "Experience" are the correct labels for their respective content. Projects are things CJK designed, built, and owns. Experience is organisations CJK worked for and roles held. The distinction is accurate, industry-standard in technical portfolios, and immediately legible to the target audiences.

Credentials at top level gives 25 certifications the visibility they earn. Legacy at top level honours the scope of the interdisciplinary practice without subordinating it.

The wrap risk analysis confirmed that the MkDocs Material framework handles the layout automatically. There is no technical objection to 7 items.

---

## Non-Goals / Constraints

- Sub-page structure within each top-level section is governed by ADR-004, not this document.
- Mobile navigation behaviour is delegated entirely to MkDocs Material's built-in hamburger implementation. No custom mobile nav is required or in scope.
- This decision does not govern footer navigation.

---

## Consequences

- KH-010 is superseded by this decision.
- All internal links, signpost cards, and cross-references must use the new labels.
- MkDocs `nav:` block in `mkdocs.yml` to be updated to reflect this order.

---

## Supersedes

KH-010 (2026-03-19) — Navigation order: Home · Work · Method · Credentials · About · Legacy.
