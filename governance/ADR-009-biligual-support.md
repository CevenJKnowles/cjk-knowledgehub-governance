---
id: ADR-009
title: "ADR | Full Site-Wide Bilingual Support — English and German"
type: adr
status: active
version: "1.0"
created: 2026-03-22
updated: 2026-03-22
provenance: human
scope: [knowledgehub]
tags: [bilingual, i18n, mkdocs, navigation, content-workflow]
related: [KH-015, KH-013, ADR-006]
ref: []
repo: []
---

# ADR | Full Site-Wide Bilingual Support — English and German

---

## Context

The CJK KnowledgeHub targets a professional audience that includes
German-speaking recruiters and hiring managers, particularly given CJK's
Berlin base and active job search in the German and European market. The
question arose whether to support German as a second language for site
visitors.

Two options were evaluated: a full bilingual site (all pages available in
both languages) and a targeted bilingual approach (selected entry-point
pages only).

---

## Decision

Full site-wide bilingual support is adopted. English is the default language.
German is the alternate language, toggled by the visitor via a language
switcher in the site navigation.

**Plugin:** `mkdocs-static-i18n`

**File naming convention:** German files use the `.de.md` suffix. Every
English `.md` file has a paired `.de.md` counterpart in the same directory.

**Content workflow:** CJK authors or approves English content. German content
is produced in the same pass by Claude and quality-gated by CJK before
commit. CJK is the final arbiter of German register and accuracy.

---

## Alternatives Considered

**Targeted bilingual (entry-point pages only)** -- rejected. When a visitor
toggles to German and encounters an untranslated page, the experience
degrades to either an English fallback or a 404. Neither is acceptable for
a site intended to signal professional rigour. Full bilingual is the only
implementation that delivers a consistent visitor experience.

**English only** -- rejected. CJK is Berlin-based and actively targeting
roles in the German and European market. A bilingual site is a meaningful
signal to German-speaking audiences and a direct demonstration of capability.

---

## Rationale

A partial bilingual approach creates language-switching gaps that degrade
the visitor experience. Full bilingual is the only implementation that
behaves predictably on every page. The maintenance overhead is manageable
because German content is produced collaboratively rather than written
independently, reducing the per-page effort to a review and approval cycle.

---

## Non-Goals / Constraints

- No additional languages beyond English and German at this stage.
- Machine translation is not used. All German content is produced by Claude
  and reviewed by CJK before commit.
- The German layer mirrors the IA skeleton (KH-013) exactly. No structural
  divergence between languages.

---

## Consequences

- Every page in the IA requires a `.de.md` counterpart.
- All future content additions are two deliverables: English and German.
- `mkdocs-static-i18n` is added to `requirements.txt` and `mkdocs.yml`.
- The language switcher appears in the site navigation on all pages.
- German files must be committed in the same PR as their English counterpart.
  Partial commits that leave a page untranslated are not permitted.

---

## Supersedes

None.

---

## Review Trigger

Revisit if a third language is proposed, or if the content maintenance
overhead becomes unsustainable.