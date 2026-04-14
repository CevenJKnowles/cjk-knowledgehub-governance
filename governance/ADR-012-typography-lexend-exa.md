---
id: ADR-012
title: Typography Update — Lexend Exa replaces Cooper Hewitt for headings
type: adr
status: locked
version: "1.0"
created: 2026-04-13
updated: 2026-04-13
provenance: human-led
scope: knowledgehub
tags: [typography, visual-design, fonts, adr]
related: [ADR-012]
ref: [VIS-004b]
repo: [cjk-knowledgehub, cjk-knowledgehub-governance]
---

> *Supersedes VIS-004b (Cooper Hewitt as heading font) as of 2026-04-13.*

# ADR-012: Typography Update — Lexend Exa replaces Cooper Hewitt for headings

---

## Status

Locked

---

## Context

VIS-004b locked Cooper Hewitt Bold/Heavy as the heading typeface for the CJK KnowledgeHub, self-hosted via `@fontsource/cooper-hewitt` woff/woff2 files at `docs/assets/fonts/cooperhewitt/`. A deferred note in that decision recorded that Cooper Hewitt read slightly condensed in the navigation at screen resolution, with a letter-spacing adjustment required during the visual polish pass.

During Session 11 (2026-04-13), CJK elected to replace Cooper Hewitt with Lexend Exa ahead of the visual polish pass rather than attempt correction via letter-spacing. Lexend Exa provides comparable weight and presence at heading sizes with improved legibility characteristics and without the condensed rendering issue observed in navigation contexts.

---

## Decision

Lexend Exa replaces Cooper Hewitt as the heading typeface across the CJK KnowledgeHub.

- Font files installed via `@fontsource/lexend-exa` and self-hosted at `docs/assets/fonts/lexendexa/`
- All `@font-face` declarations for Cooper Hewitt removed from `docs/assets/stylesheets/custom.css`
- All heading `font-family` references updated from `'Cooper Hewitt'` to `'Lexend Exa'`
- Cooper Hewitt font files retained at `docs/assets/fonts/cooperhewitt/` pending confirmation of clean build and visual review; to be removed in a subsequent cleanup commit
- Body font (Barlow Regular) and code font (Hack Regular) unchanged

---

## Consequences

- Navigation condensed rendering issue resolved without requiring letter-spacing correction
- VIS-004b is archived and superseded by this record
- TPL-001 v2.0 `scope` field convention applied to this ADR
- Cooper Hewitt files to be removed in a follow-up cleanup commit once visual review is confirmed

---

*End of ADR-012*
