---
id: ADR-004
title: "ADR | Typography — Headings, Body, and Code Fonts"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [visual-design, typography, fonts]
related: [ADR-005]
ref: []
repo: []
---

# ADR | Typography — Headings, Body, and Code Fonts

---

## Context

The KnowledgeHub requires a typography system covering three distinct roles: headings, body and UI text, and code and monospace output. The system must satisfy the following brief:

- Highly accessible letterforms
- Technical character — consistent with engineering drawings, instrument panels, or systems documentation
- Futuristic without being theatrical
- Serious without being flat
- All fonts must be OFL licensed and freely usable — no corporate IP

An earlier logged decision (VIS-004, 2026-03-20) recorded `Inter` and `JetBrains Mono` as the locked choices. That entry was identified as an error — the conversation never took place. VIS-004 was voided and this decision supersedes it.

---

## Decision

| Role | Font | Weight |
|---|---|---|
| Headings | Cooper Hewitt | Bold / Heavy |
| Body / UI text | Barlow | Regular (400) |
| Code / monospace | Hack | Regular (400) |

All three fonts are licensed under the SIL Open Font License (OFL) and are freely usable without corporate IP restriction.

---

## Alternatives Considered

**Space Grotesk (body)** — evaluated and rejected. Geometric and technically credible, but the lowercase `g` and `y` carry deliberately quirky descenders that read as theatrical in a technical portfolio context. Not the right register.

**Lexend (body)** — evaluated. Accessibility-first, warm and open. Rejected in favour of Barlow on balance grounds — Lexend is designed to recede, where the brief requires the body to hold its own alongside heavy headings.

**DM Sans (body)** — evaluated against Barlow via rendered specimen. DM Sans is optically corrected to disappear at reading size. Rejected because the brief requires balanced weight between heading and body, not a receding body font.

**Exo 2 (body)** — considered as a Space Grotesk alternative. Explicitly technical-futuristic DNA. Not selected — Barlow's signage geometry and geometric grotesque roots were a closer fit to the brief.

**IBM Plex Sans (body)** — considered. Strong technical drawing DNA, warm enough not to be cold. Not selected — Barlow was preferred after specimen comparison.

**Inter (body)** — excluded. Google / corporate IP concerns raised by CJK.

**Open Sans / Source Sans Pro (body)** — excluded. Corporate IP (Google / Adobe).

**Tahoma (body)** — excluded. Microsoft proprietary, not freely usable.

**JetBrains Mono (code)** — excluded. Considered in the erroneously logged VIS-004. Conversation never took place; excluded from consideration in the actual decision session.

**OpenDyslexic (body)** — evaluated. Maximum accessibility. Reads as unconventional in a technical portfolio context and would work against the tone.

---

## Rationale

**Cooper Hewitt** — released by the Smithsonian Cooper Hewitt museum under OFL. Geometric humanist. The Heavy and Bold weights carry significant authority and visual confidence. Seven weights available, allowing consistent use across heading levels.

**Barlow** — OFL, inspired by California highway signage and early 20th century geometric grotesques. Has enough geometric confidence to hold its own alongside a heavy heading weight without competing. The rendered specimen confirmed balance against Cooper Hewitt. Not so condensed as to feel compressed; not so wide as to feel soft.

**Hack** — designed specifically for code editors and terminals. Has genuine CRT-terminal character without being retro-pastiche. Closest match to the brief's "old CRT monitor" reference in a code context. OFL.

---

## Non-Goals / Constraints

- This decision covers web typography only. Print and PDF contexts may differ.
- Font weights other than those specified above are not locked — they may be used as needed within each font family.
- Web font delivery via Google Fonts CDN is acceptable given that OFL ownership is independent of Google hosting.

---

## Consequences

- All KnowledgeHub pages use this font stack.
- Implementation via `docs/assets/stylesheets/custom.css` per VIS-005.
- Google Fonts `@import` or `<link>` for Cooper Hewitt, Barlow, and Hack to be configured in `mkdocs.yml`.

---

## Supersedes

VIS-004 (voided 2026-03-20 — logged in error, conversation never took place).
