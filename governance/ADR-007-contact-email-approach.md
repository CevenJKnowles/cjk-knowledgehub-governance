---
id: ADR-007
title: "ADR | Contact Email Approach"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [contact, privacy, anti-spam, about]
related: [ADR-008]
ref: []
repo: []
---

# ADR | Contact Email Approach

---

## Context

The KnowledgeHub requires a contact mechanism on the About page. A raw email address in HTML source is trivially harvested by spam bots. The CV email address (`ceven@cevenknowles.com`) is not for public-facing use. A dedicated contact email address is required.

The contact mechanism must balance three competing constraints:
- Accessibility for legitimate human contacts (recruiters, hiring managers, collaborators)
- Protection against automated spam harvesting
- Minimal friction for the reader

---

## Decision

Two-layer approach:

1. **Email obfuscation** — the contact email address is assembled client-side via JavaScript and never present as a raw string in HTML source. Displayed as readable text to humans. Not accessible to standard bot scraping.

2. **Formspree contact form** — the primary contact mechanism. No email address is exposed. The form submits to Formspree's service, which forwards to the designated inbox. Free tier is sufficient for expected volume.

Both mechanisms appear on the About page. The obfuscated address serves readers who prefer to copy the address directly into their mail client. The form serves readers who want to send a message without leaving the site.

The dedicated public-facing contact email address is to be created by CJK before implementation. Address TBC.

---

## Alternatives Considered

**Raw mailto link** — rejected. The address is present in HTML source and trivially harvested.

**Mailto link with display text only** — rejected. The `href` attribute still contains the raw address and is scraped by sophisticated bots.

**Email address rendered as PNG image** — evaluated. Bot-resistant but inaccessible to screen readers and cannot be copied. Maintenance overhead if address changes. Rejected.

**Cloudflare Turnstile protected form** — evaluated. More robust bot protection. Additional setup complexity and a CAPTCHA creates friction for legitimate users. Rejected in favour of the simpler Formspree approach for initial launch. May be reconsidered if spam volume becomes a problem.

**No email at all, form only** — evaluated. Maximally protective. Rejected because some users, particularly technical reviewers and senior hiring managers, prefer direct email contact over form submissions.

---

## Rationale

The combination of obfuscation and a form covers both contact preferences without fully exposing the address. Formspree's free tier requires no backend and integrates cleanly with a static MkDocs site. The obfuscation approach eliminates the majority of bot harvesting without adding CAPTCHA friction.

---

## Non-Goals / Constraints

- This decision covers the About page only. No contact mechanism elsewhere on the site.
- The CV email address (`ceven@cevenknowles.com`) must never appear on the public-facing site.
- No phone number anywhere on the site per MP-001.
- The dedicated contact address is a pending action item — implementation is blocked until it is created.

---

## Consequences

- About page requires a small JavaScript snippet for client-side address assembly.
- Formspree account setup required before launch.
- Contact email address must be created and supplied to implementation before this can be completed.

---

## Supersedes

None.

---

## Review Trigger

Review if spam volume becomes problematic after launch. Cloudflare Turnstile is the natural upgrade path.
