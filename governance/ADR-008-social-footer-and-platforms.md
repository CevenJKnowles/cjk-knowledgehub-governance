---
id: ADR-008
title: "ADR | Social Footer and Platform List"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [social, footer, navigation, presence]
related: [ADR-007]
ref: []
repo: []
---

# ADR | Social Footer and Platform List

---

## Context

The KnowledgeHub requires a consistent social presence mechanism across all pages, with contextual surfacing on pages where specific platforms are directly relevant. MkDocs Material provides a native social links block in the footer via `extra.social` in `mkdocs.yml`, rendering as icon links on every page at no implementation cost.

The platform list must reflect CJK's active, credible, and professional presence only. Platforms with thin, dormant, or personal content are excluded.

---

## Decision

### Implementation

MkDocs Material native `extra.social` block in the site footer. Present on every page automatically. No custom implementation required.

### Confirmed Platform List

| Platform | Rationale |
|---|---|
| GitHub | Primary artefact host. Non-negotiable. |
| LinkedIn | Active profile, optimised. Non-negotiable for job search. |
| Bluesky | Active AI and technical practitioner community. Growing presence in CJK's target professional context. |
| Behance | Professional visual and creative work archive. Directly relevant to Legacy section. |
| Instagram | Professional visual work account. Complements Behance. Contextually relevant to Legacy. |
| Stack Overflow | Articles in production at time of decision. Profile active. |

### Excluded Platforms

| Platform | Reason |
|---|---|
| Newsletter | Excluded entirely. No issues published. A newsletter link without content signals intention without evidence. |
| Hugging Face | Not yet relevant. Revisit if model-level work is published. |

### Contextual Placement

In addition to the footer baseline, social links are surfaced contextually on:

- **Home** — primary landing page, social proof signals appropriate
- **About** — biographical context, LinkedIn and GitHub natural here
- **Legacy** — Behance and Instagram linked directly in body content per VIS-007

Contextual placement surfaces only the platforms directly relevant to each page. Full icon block is not repeated verbatim on every contextual page.

---

## Alternatives Considered

**Custom social block in page header** — evaluated. Would increase visibility. Rejected — the footer is the established convention for persistent social links and is where readers expect to find them. Header placement would be visually intrusive.

**Social links on every page in body content** — evaluated. Excessive. Dilutes the contextual relevance of links on specific pages. Rejected.

**Include newsletter link as placeholder** — rejected. An empty or not-yet-live subscription link signals intention without delivery. Excluded until at minimum one issue is published.

---

## Rationale

The footer baseline ensures every page on the site surfaces social links passively without interrupting content. Contextual surfacing on three specific pages gives the most relevant links prominence where they add direct value. The platform list reflects active, professionally relevant presence only — no padding.

---

## Non-Goals / Constraints

- Platform list is not exhaustive of all platforms CJK may use. It reflects what is appropriate for public professional surfacing at time of launch.
- Stack Overflow link is included on the basis that articles are in active production. If articles are not published before site launch, this should be reviewed.
- This decision does not govern the visual styling of social icons — that is a CSS implementation detail.

---

## Consequences

- `extra.social` block to be configured in `mkdocs.yml` with the six confirmed platforms.
- MkDocs Material supports native icons for GitHub, LinkedIn, and Behance. Bluesky, Instagram, and Stack Overflow may require custom SVG icon configuration.
- Contextual link placement on Home, About, and Legacy pages to be implemented per content population phase.

---

## Supersedes

None.

---

## Review Trigger

- Stack Overflow: review before launch if articles remain unpublished.
- Newsletter: revisit when first issue is published.
- Hugging Face: revisit if model-level portfolio work is published.
