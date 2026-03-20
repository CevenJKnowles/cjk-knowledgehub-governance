---
id: ADR-006
title: "ADR | Information Architecture Skeleton"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [information-architecture, content-structure]
related: [ADR-005]
ref: []
repo: []
---

# ADR | Information Architecture Skeleton

---

## Context

With the top-level navigation locked (ADR-003), the content structure beneath each section requires definition before implementation begins. The IA must serve four distinct audiences: curious tinkerers, recruiters and hiring managers, senior managers and directors, and technical specialists. Content must be layered so each audience finds what they need without noise.

The KnowledgeHub is itself a portfolio artefact. Its architecture is a demonstration of CJK's systems thinking and documentation rigour — not merely a presentation layer.

---

## Decision

### Home

Single landing page. Hero statement, headline, positioning line. Signpost cards linking to the six other sections. Contextual social links. No long-form content — the page leads, it does not explain.

---

### Projects

Dedicated pages for each artefact:

- **IO-III Architecture** — governed LLM infrastructure and systems design project. Full write-up, phase status, ADR-first methodology, GitHub link.
- **Prompt Pattern Library** — canonical taxonomy and atomic pattern library. Taxonomy overview, schema architecture, development status note, GitHub link.
- **cjk-knowledgehub-governance** — positioned as a live artefact demonstrating documentation practice, governance rigour, and ADR methodology.
- **Agentic-Applications fork** — brief write-up, context, GitHub link.

---

### Experience

- **Simpleshow** — Conceptor and Project Manager, Freelance, Nov 2020 – Dec 2024. Four bullets per KH-004.
- **Interdisciplinary Media Designer** — Self-employed, International, May 1999 – Dec 2024. Selected bullets. 500 projects figure retained here per LI-004.
- **LUDWIG Bar / Gallery / Venue** — Co-owner and Operator, Berlin-Neukölln, Dec 2015 – Sep 2019. Four bullets.

---

### Method

- **How I work** — ADR-first methodology, deterministic design philosophy, constraint-as-feature framing. First-person authorial register.
- **Architecture Decision Records** — what they are, why they matter, link to governance repo as a live example.
- **Tools and environment** — Git, Bash, VS Code, MkDocs, JupyterLab, Arch Linux. Python not foregrounded per ADR-011.

---

### Credentials

- Full list of 25 certifications, grouped by domain. Domains drawn from CV groupings: Statistical and Mathematical Foundations, AI Engineering and Governance, and any additional domains from the full list (Bildungsgutschein Anlage 6 is the authoritative source).
- Education: excluded until a formal qualification is held.

---

### About

Single page. Profile statement adapted for web register. Positioning headline. Location: Berlin, remote-first. Contact: obfuscated email plus Formspree form. No phone number, no physical address per MP-001. Contextual social links.

---

### Legacy

Overview of 26-year interdisciplinary practice spanning digital, web, video, and live media formats. Functions both as a standalone section and as a reference target from other pages where past work is contextually relevant. Old artefacts included where available and appropriate. Behance and Instagram linked in body content. Contextual social links.

---

## Alternatives Considered

**Merge Projects and Experience under "Work"** — the original KH-010 structure. Rejected in ADR-003 — conflates owned artefacts with employment history.

**Place Credentials under About** — evaluated. Rejected because Credentials is verified external evidence of technical competence, not biographical context. It warrants top-level visibility for a technical audience.

**Include Education under Credentials** — deferred. No formal qualification currently held. Education section to be added when applicable.

**Embed Legacy under About** — evaluated. Rejected. Legacy covers 26 years of interdisciplinary practice and functions as a reference target from multiple other pages. It has sufficient content and navigational importance to stand independently at top level.

---

## Rationale

The skeleton reflects the layered audience model: Home and About serve all audiences; Projects and Credentials serve technical specialists and hiring managers directly; Experience provides context; Method signals working practice and architectural rigour; Legacy contextualises the full career arc.

Each section is independently navigable and self-contained. No section requires reading another to make sense.

---

## Non-Goals / Constraints

- This ADR defines structure only. Content, copy, and visual treatment are out of scope here.
- The KnowledgeHub itself (this governance repo and the main repo) is referenced within Projects but does not appear as a separate navigation item — the site is itself the artefact.
- No content is written or committed until CJK confirms each section individually.

---

## Consequences

- `mkdocs.yml` nav block to reflect this skeleton exactly.
- Page stubs to be created for each section and sub-page before content population begins.
- Credentials page structure pending full 25-certification list from Bildungsgutschein Anlage 6.

---

## Supersedes

None.

---

## Review Trigger

Revisit if a significant new project artefact is created that warrants its own top-level section, or if the audience model changes materially.
