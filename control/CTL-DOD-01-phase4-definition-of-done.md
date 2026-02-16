---
id: CTL-DOD-01
layer: control
type: DOD
phase: P4
status: active
created: 2026-02-12
updated: 2026-02-16
---
---
# Phase 4 — Definition of Done (DoD)  
## Per Page Type (Canonical)

**Project:** CJK_Knowledgehub  
**Phase:** 4 (Implementation & Content Build)  
**Status:** Governing  
**Depends On:** Phase 1, Phase 2, Phase 3 (all locked)

---

## Global DoD (Applies to All Page Types)

A page is **not complete** unless all items below are satisfied:

- [ ] Declares exactly one canonical `type`
- [ ] Declares exactly one canonical `domain`
- [ ] YAML front-matter is present, valid, and minimal
- [ ] Page purpose can be stated in **one sentence**
- [ ] Uses only approved section vocabulary
- [ ] Scope is bounded; no “just in case” content
- [ ] Explicitly acknowledges limits, tradeoffs, or exclusions
- [ ] No aspirational, speculative, or educational framing
- [ ] Improves recruiter trust on first read
- [ ] Can be defended verbally in a professional review

Failure on any item blocks approval.

---

## Page Type: `profile`

**Intent:** Orientation, positioning, and reading contract.

### Required
- [ ] Clear professional positioning
- [ ] Capability summary grounded in evidence (not claims)
- [ ] Navigation guidance for different reader paths
- [ ] Tone is confident, restrained, non-promotional

### Prohibited
- [ ] Personal narrative or learning journey
- [ ] Tool lists or skills dumping
- [ ] Repetition of Career Trajectory content

### DoD Confirmation
- [ ] Frames interpretation of all downstream content correctly
- [ ] Contains no placeholders or promises

---

## Page Type: `case-study` (Prompt Engineering only)

**Intent:** Applied evidence of judgment and evaluation.

### Required
- [ ] Problem clearly defined and bounded
- [ ] Constraints stated before solutions
- [ ] Design decisions explicitly justified
- [ ] Evaluation method stated and applied
- [ ] Tradeoffs and failure modes acknowledged

### Prohibited
- [ ] Prompt collections without context
- [ ] Tool-first or technique-first framing
- [ ] “Best practices” tone

### DoD Confirmation
- [ ] Defensible in an interview discussion
- [ ] Adds unique signal relative to other case studies

---

## Page Type: `workflow`

**Intent:** Operational system design and recovery thinking.

### Required
- [ ] Clear trigger or initiating condition
- [ ] Structured flow or stages
- [ ] Explicit decision points
- [ ] Failure modes and recovery strategies
- [ ] Takeaways grounded in experience

### Prohibited
- [ ] Generic process diagrams
- [ ] Theoretical or idealized flows
- [ ] Tool tutorials

### DoD Confirmation
- [ ] Justified by at least one case study
- [ ] Demonstrates operational maturity

---

## Page Type: `documentation`

**Intent:** Documentation as a professional capability.

### Required
- [ ] Documentation intent clearly stated
- [ ] Structure and scope decisions explained
- [ ] Governance or maintenance model described
- [ ] Evidence of restraint and judgment

### Prohibited
- [ ] How-to guides or instructional tone
- [ ] Exhaustive or encyclopedic coverage
- [ ] Redundant restatement of workflows

### DoD Confirmation
- [ ] Demonstrates clarity, not verbosity
- [ ] Anchored to a concrete workflow

---

## Page Type: `context` (Career Trajectory)

**Intent:** Explain continuity and transferability.

### Required
- [ ] Clear professional through-line
- [ ] Transferable capabilities grounded in evidence
- [ ] Collaboration posture articulated
- [ ] Explicit boundaries and limits

### Prohibited
- [ ] Role shopping or future casting
- [ ] Rewriting the Profile page
- [ ] Repetition of CV-style lists

### DoD Confirmation
- [ ] Synthesizes prior domains coherently
- [ ] Explains *why* the evidence fits together

---

## Page Type: `reference` (Appendix)

**Intent:** Verification and lookup only.

### Required
- [ ] Structured, scannable presentation
- [ ] Minimal prose
- [ ] Clear categorization
- [ ] Accurate and current entries

### Prohibited
- [ ] Narrative explanation
- [ ] New claims or interpretations
- [ ] Overexposure in navigation

### DoD Confirmation
- [ ] Strengthens trust without distracting
- [ ] Entirely optional for first-time readers

---

## Media DoD (All Page Types)

If a page includes media:

- [ ] Media directly supports a specific point in the text
- [ ] Media is referenced explicitly in context
- [ ] Media carries no standalone meaning
- [ ] Media can be removed without breaking logic

Decorative or unreferenced media fails DoD.

---

## Final Approval Rule

A page is **approved** only when:

- all applicable DoD items are satisfied,
- Ceven explicitly confirms approval,
- and no unresolved objections remain.

Silent approval is invalid.

---

**End of Phase 4 — Definition of Done**
