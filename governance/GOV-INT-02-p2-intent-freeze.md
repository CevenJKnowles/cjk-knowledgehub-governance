```yaml
id: GOV-INT-02
layer: GOV
type: INT
phase: P2
status: frozen
created: 2026-02-08
updated: 2026-02-12
```
# Phase 2 | Architecture & Presentation Intent Freeze (Canonical)

**Status:** Locked  
**Phase:** 2 (Architecture Planning)  
**Supersedes:** All prior architectural assumptions  
**Depends on:** Phase 1 — Intent Freeze

---

## 1. Purpose of Phase 2

Phase 2 translates the **frozen intent** of Phase 1 into a **coherent public-facing architecture**, defining:

- how content is organized,
- how it is presented,
- how it is navigated,
- and how long-term coherence is maintained,

**before** any files, folders, visuals, or implementations exist.

Phase 2 is conceptual and structural only.

---

## 2. Canonical Content Domains (Final)

The KnowledgeHub is structured around exactly **six domains**:

1. **Profile**  
   Professional identity, positioning, and interpretive framing.

2. **Prompt Engineering**  
   Exactly **three** applied prompt engineering case studies.

3. **Workflows**  
   Operational systems, process design, and recovery-oriented thinking.

4. **Documentation**  
   Documentation as a professional capability (structure, scope, governance).

5. **Career Trajectory**  
   Structural explanation of professional continuity, transferability, and collaboration posture.

6. **Appendix**  
   Reference material: certifications, skills, tools, and metadata indices.

No additional domains are permitted without revising this document.

---

## 3. Top-Level Information Architecture (Phase 2.1)

### IA Model
**Model 1 — Portfolio-First** is locked.

### Primary Entry Point
- **Profile** is the default landing page for all users.

### Primary Navigation Order
1. Profile  
2. Prompt Engineering  
3. Workflows  
4. Documentation  
5. Career Trajectory  
6. Appendix

Navigation prioritizes **evidence and clarity** over completeness.

---

## 4. Reading Paths (Conceptual, Not Gated)

The KnowledgeHub supports **three intended reading paths**, implemented via emphasis, order, and signposting — not user detection.

### Path A — Recruiter Fast Path (60–120 seconds)
- Profile
- Prompt Engineering (scan 1 case study)
- Career Trajectory
- Appendix (optional verification)

### Path B — Hiring Manager Path (5–10 minutes)
- Profile or Prompt Engineering
- Prompt Engineering (2–3 case studies)
- Workflows (1–2)
- Documentation (1 example)
- Career Trajectory
- Appendix

### Path C — Technical Reviewer Path (Selective depth)
- Prompt Engineering or Workflows
- Workflow → Documentation cross-links
- Appendix (validation only)

Intentional friction is applied to prevent premature depth and noise.

---

## 5. Content Presentation System (Phase 2.3)

### Core Principle
> **Consistency without rigidity.**

Readers should learn how to read the system once.

---

### 5.1 Canonical Page Types (Final)

Every page must declare exactly one page type:

- `profile` — Orientation & framing
- `case-study` — Applied evidence (Prompt Engineering only)
- `workflow` — Operational system design
- `documentation` — Documentation capability proof
- `context` — Career Trajectory content
- `reference` — Appendix & indices

---

### 5.2 Global Section Vocabulary (Stable Meanings)

The following section concepts have invariant meaning across the KnowledgeHub:

- Intent  
- Context  
- Problem / Trigger  
- Constraints  
- Design Decisions  
- Execution / Structure  
- Evidence / Evaluation  
- Tradeoffs / Limits  
- Outcome / Takeaways  
- References  

Not all pages use all sections.  
Omission is intentional, not accidental.

---

### 5.3 Domain-Specific Emphasis Rules

- **Prompt Engineering:**  
  Problem → Constraints → Decisions → Evaluation → Tradeoffs

- **Workflows:**  
  Trigger → Structure → Decision Points → Failure & Recovery → Takeaways

- **Documentation:**  
  Intent → Structure → Scope Decisions → Governance → Maintenance

- **Career Trajectory:**  
  Context → Continuity → Transferable Capabilities → Collaboration Posture → Boundaries

- **Profile:**  
  Intent → Positioning → Capability Summary → Navigation Guidance

- **Appendix:**  
  Reference-only, minimal prose, structured indices

---

## 6. Metadata & Continuity Schema (Phase 2.4)

### 6.1 YAML Front-Matter
- YAML front-matter is used **globally**
- Purpose: structure, continuity, and future optional automation
- Not used for SEO or verbosity

---

### 6.2 Global Metadata Fields

**Required (all pages):**
- `title`
- `type` (canonical page type)
- `domain` (one of six domains)
- `status` (`canonical | evolving | reference`)

**Optional (controlled):**
- `audience` (`recruiter | hiring-manager | technical | reference`)
- `confidence-level` (`production-ready | well-tested | exploratory`)
- `last-reviewed` (governance only)

---

### 6.3 Domain-Specific Metadata (Minimal)

- **Prompt Engineering**
  - `problem-class`
  - `evaluation-method`

- **Workflows**
  - `workflow-scope`
  - `failure-modes-covered`

- **Documentation**
  - `documentation-type`
  - `maintenance-model`

- **Appendix**
  - `category`
  - `issuer` (certifications)

No additional metadata fields without explicit review.

---

### 6.4 Tag Governance

- Tags are allowed but strictly governed
- Tags describe **capability, method, or context**
- No duplication with domain or type
- No buzzwords, no tool sprawl

---

### 6.5 Cross-Linking Rules

Allowed:
- Case study → workflow
- Workflow → documentation
- Certification → applied evidence

Disallowed:
- Link farms
- Undirected “see also” lists

Rule:
> If the link’s purpose cannot be stated in one sentence, it does not exist.

---

## 7. Governance Rules (Phase 2.6)

### Content Admission
New content is added only if:
1. It fits one of the six domains
2. It matches a canonical page type
3. It satisfies Phase 1 success criteria
4. Its purpose is clear in one sentence

---

### Revision Triggers
- Better evidence replaces weaker evidence
- Insight changes conclusions
- Role alignment changes

Not triggered by:
- time passing
- trends
- discomfort with wording

---

### Exception Handling
Uncertain content must pass **2 of 3**:
- Evidence value
- Role signal
- Interpretability

All exceptions are explicit and revisitable.

---

### Pause / Resume Protocol
On pause:
- No partial drafts
- Leave a clear “next intended action”

On resume:
- Re-read Phase 1 Intent Freeze
- Re-read this Phase 2 Intent Freeze
- Continue without reinterpretation

---

## 8. Phase 2 Closure

With this document:
- Architecture is locked
- Presentation logic is fixed
- Metadata system is defined
- Navigation intent is frozen
- Drift prevention is active

Phase 2 is formally complete.

---

**End of Phase 2 Intent Freeze**
