---
id: LOG-007
title: Session 11 — About, Legacy, Visual Polish, Font Switch
type: log
status: active
version: "1.0"
created: 2026-04-13
updated: 2026-04-13
provenance: ai-assisted
scope: knowledgehub
tags: [session-log, content, visual-design, about, legacy, lexend-exa]
related: [LOG-006, ADR-012, SNP-CUR-01]
ref: [KH-018, COP-001]
repo: [cjk-knowledgehub, cjk-knowledgehub-governance]
---

# LOG-007: Session 11 — About, Legacy, Visual Polish, Font Switch

Date: 2026-04-13
Session: 11

---

## Summary

Four workstreams completed this session. All content sections are now
committed. The full site content layer is complete. Visual polish pass
executed across two rounds of CSS iteration. Font switched from Cooper
Hewitt to Lexend Exa.

---

## Decisions Locked

### ß convention
German copy uses ß throughout. `einschließlich`, `Maßstab`, etc.
All future German files follow this convention.

### TPL-001 v2.0
`scope` field formally documented in TPL-001. Committed by CJK.
Open item from Session 6 resolved.

### ADR-012 — Lexend Exa replaces Cooper Hewitt
VIS-004b superseded. Lexend Exa installed via `@fontsource/lexend-exa`,
self-hosted at `docs/assets/fonts/Lexend_Exa/`. All heading font
references updated in `custom.css`. Cooper Hewitt files retained pending
cleanup commit.

---

## Content Committed — KnowledgeHub Repo

### About section
- `docs/about/index.md` — v0.3
- `docs/about/index.de.md` — v0.1

First-person narrative. Covers Berlin relocation (2004), citizenship
(2010), career arc from photography through video, internet, agency
work, AI systems. Audience: recruiters, senior engineers, marginalised
communities. Authentic voice. No corporate inflation.

### Legacy section
- `docs/legacy/index.md` — v0.5
- `docs/legacy/index.de.md` — v0.1

Chronological essay with links. Covers: 1999 livestreams and Ana Voog
collaboration; Anderecast anthology series (200+ episodes, 10,000
viewers/episode, 2006--2008); Hinausgehen audiovisual sonata at
Länsmuseum Jönköping 2012; Cerusmedia music video and live visuals
practice including Lesley Rankine/Ruby and The Opiates
(Billie Ray Martin and Robert Solheim); ELECTROSEXUAL Best Music
Video win at Singapore International Short Film Festival 2021;
LUDWIG Bar/Gallery/Venue 2016--2019 including CHAOSTROPHY exhibition;
public record summary with press links.
LUDWIG section standalone paragraph as specified.

---

## Visual Polish — custom.css and mkdocs.yml

### Font switch (ADR-012)
Cooper Hewitt `@font-face` declarations removed. Lexend Exa declarations
added covering weights 100--900. All heading font-family references
updated to `'Lexend Exa'`.

### pymdownx.emoji extension
Added to `mkdocs.yml` markdown_extensions block. Fixes all
`:material-icon-name:` references rendering as literal text in content.

### Social icons updated to Simple Icons
All footer social icons switched to `simple/` prefix for cohesion.
YouTube and Substack added.
Full social list: GitHub, LinkedIn, Bluesky, Instagram, Behance,
Stack Overflow, YouTube, Substack.

### Sidebar social + contact widget
`overrides/partials/nav.html` created. Social icons with inline SVGs
injected below nav. Contact email displayed as plain selectable text
(not a link) to prevent spam. CSS rules added for widget layout and
hover states.

### Nav tab colours
Light mode: inactive `#efefef`, active/hover `#ff6700`.
Dark mode: inactive `#ff6700`, active/hover `#efefef`.

### UI icon colours
Language switcher and day/night toggle: `#ff6700` in both modes.

### Repo link visibility
`.md-source__repository` and `.md-source__facts` colour rules added
for light mode visibility.

### Logo size
`.md-logo img` height set to `2.5rem`.

---

## Governance Files Produced

- `governance/ADR-012-typography-lexend-exa.md` — v1.0
- `snapshots/LOG-007-knowledgehub-about-legacy-visual-polish-2026-04-13.md` — v1.0
- `snapshots/SNP-CUR-01-current-state.md` — v2.0

---

## Open Items

| Item | Status |
|---|---|
| Cooper Hewitt font files cleanup commit | Pending — remove `docs/assets/fonts/cooperhewitt/` once confirmed |
| Stack Overflow profile URL | Needs verification before publish |
| Contact form (Formspree) | Not yet implemented — deferred |
| Visual polish pass round 3 | Pending CJK review of live site |

---

## Next Session Anchor

All content sections committed. Site is in a publishable state pending:
1. Final visual review on live/staging
2. Cooper Hewitt cleanup commit
3. Stack Overflow URL verification
4. Contact form decision (Formspree vs email-only)
5. Domain redirect cevenknowles.com (Phase 6)

---

*End of LOG-007*
