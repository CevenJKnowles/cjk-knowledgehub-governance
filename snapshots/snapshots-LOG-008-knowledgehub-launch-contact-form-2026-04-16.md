---
id: LOG-008
title: Session 12 Log — Launch, Contact Form, Footer Polish
type: log
status: final
version: v1.0
created: 2026-04-16
updated: 2026-04-16
provenance: session-12
scope: cjk-knowledgehub
tags: [launch, domain, contact-form, footer, css, deployment]
related: [ADR-012, CON-001, CON-002]
ref: ~
repo: cjk-knowledgehub-governance
---

## Summary

Session 12 completed Phase 6 (domain redirect) and all remaining pre-launch
items. A contact form was implemented and footer styling finalised. The site is
fully live at https://cevenknowles.com.

---

## Workstreams Completed

### Phase 6 — Domain Redirect

- DreamHost DNS configured: four GitHub Pages A records and one CNAME for `www`
- `docs/CNAME` created with value `cevenknowles.com`
- GitHub Pages custom domain set; HTTPS enforced
- Post-launch fix: `site_url` in `mkdocs.yml` updated to `https://cevenknowles.com/`
  (internal links were resolving to `/cjk-knowledgehub/` path)
- Post-launch fix: `CNAME` moved from repo root to `docs/` so `mkdocs gh-deploy`
  includes it in build output; GitHub Pages custom domain re-entered after redeploy

### Pre-Launch Cleanup

- `docs/assets/fonts/cooperhewitt/` removed from repo (superseded by Lexend Exa,
  ADR-012)
- Stack Overflow profile URL corrected to:
  `https://stackoverflow.com/users/31796358/ceven-jupiter-knowles`

### Contact Form — Web3Forms

- Formspree replaced by Web3Forms on GDPR grounds (US data processing risk for
  EU-based operator)
- Form placed in sidebar below social icons; always visible
- Fields: name, email, message
- Thank-you redirect: `https://cevenknowles.com/contact/thankyou/`
- `docs/contact/thankyou.md` created
- Plain text email `hello@cevenknowles.com` removed from sidebar

### Footer and Sidebar Polish

- `mkdocs.yml`: `copyright` field set to `© 2026 | Ceven Jupiter Knowles`
- `custom.css`: MkDocs attribution hidden; footer social icons set to `#ff6700`
- `custom.css`: sidebar scrollbar hidden; bottom padding set to `10rem` to clear
  footer over contact form
- `custom.css`: "Get in touch" heading styled in Lexend Exa, no all-caps,
  `#ff6700` in dark mode (`[data-md-color-scheme="slate"]`)

---

## Files Changed

### cjk-knowledgehub

- `docs/CNAME` — moved from root; value `cevenknowles.com`
- `mkdocs.yml` — `site_url`, `copyright` updated
- `overrides/partials/nav.html` — Stack Overflow URL; Web3Forms form; email removed
- `docs/assets/stylesheets/custom.css` — form styles, scrollbar, footer, heading
- `docs/contact/thankyou.md` — thank-you page v1.0

### cjk-knowledgehub-governance

- `snapshots/LOG-008-knowledgehub-launch-contact-form-2026-04-16.md` — v1.0
- `snapshots/SNP-CUR-01-current-state.md` — v3.0

---

## Open Flags

None.