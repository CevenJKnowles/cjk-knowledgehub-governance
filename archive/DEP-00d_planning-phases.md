```yaml
id: DEP-00d_planning-phases
layer: planning
type: structural-map
phase: X
status: depreciated
created: 2026-02-16
updated: 2026-02-16
```
---
# GitHub & Public-facing GitPage Redesign  

---
---
# ⚠ Deprecated
Superseded by: PLN-MAP-01-project-workflow.md
Date: 2026-02-16

---

### Planning Phases (Canonical v1.0)

---

## Phase 1 — Repo Audit & Positioning Analysis

### Objective
Establish a clear, evidence-based understanding of the **current state of the repository ecosystem** and its suitability for recruiter- and hiring-manager-facing use, without inflating skills, roles, or claims.

This phase answers:
- What exists?
- What is strong?
- What is risky?
- What is mispositioned?

No changes are made in this phase. This is analysis only.

---

### Core Activities

- Inventory all existing repositories and major sub-projects
  - CJK KnowledgeHub (current)
  - Prompt Pattern Library
  - Io Architecture / Io Persona Blueprint
  - Supporting notebooks, experiments, drafts

- Classify each item by **readiness level**
  - Public-ready (can be shown as-is or with minimal framing)
  - Conditionally public (strong, but needs scope clarification or reframing)
  - Internal-only (valuable, but not recruiter-facing)
  - Archive / legacy (kept for history, not positioning)

- Evaluate each item against **contemporary professional standards**
  - Clarity of purpose
  - Evidence vs claims
  - Scope discipline
  - Documentation quality
  - Signal-to-noise ratio

- Cross-check alignment with target roles
  - Prompt Engineer / Prompt Specialist
  - AI Workflow Specialist
  - Technical Documentation / GenAI Documentation Engineer
  - QA / evaluation / governance-adjacent roles

---

### Explicit Non-Goals

- No refactoring
- No rewriting
- No deletions
- No aesthetic decisions

This phase is deliberately conservative.

---

### Outputs

- A written audit summary (can be bullet-based)
- A clear classification of assets by readiness and risk
- A list of **what must not be shown publicly yet**
- A short list of **high-signal assets worth building around**

---

### Reasoning

- Prevents accidental résumé inflation
- Prevents burying strong work under weak or unfinished material
- Creates shared ground truth for all later decisions
- Reduces emotional and cognitive load by replacing ambiguity with structure

This phase makes every later phase faster.

---

## Phase 2 — Architecture Planning (Conceptual)

### Objective
Design the **conceptual architecture** of the GitHub repository and public GitPage before touching files, folders, or content.

This phase answers:
- Where does information live?
- For whom?
- At what level of abstraction?
- With what boundaries?

---

### Core Architecture Principles

- Separation of concerns
  - Public narrative ≠ evidence ≠ R&D
- Evidence-first ordering
  - Artifacts precede claims
- Explicit scope boundaries
  - What the KnowledgeHub is
  - What it is not

---

### Conceptual Layers (Not File Structure Yet)

- Public Signal Layer (GitPage)
  - Curated, low-volume, high-clarity
  - Designed for recruiters and hiring managers
  - Emphasizes judgment, outcomes, and scope discipline

- Portfolio Evidence Layer (GitHub-facing)
  - Case studies
  - Prompt engineering showcases
  - Evaluations, workflows, failure analysis
  - Linked from the GitPage, not dumped into it

- Foundations & R&D Layer
  - Prompt Pattern Library (full)
  - Io Architecture
  - Experiments, notes, drafts
  - Explicitly not recruiter-facing

---

### Key Architectural Decisions

- What appears on the GitPage vs what is only linked
- How many clicks a reviewer needs to see evidence
- How to avoid overwhelming non-technical reviewers
- How to keep technical depth accessible but optional

---

### Outputs

- A written conceptual map of layers and flows
- Clear inclusion/exclusion rules for each layer
- Agreement on what types of artifacts belong where
- A shared mental model for future structure decisions

---

### Reasoning

- Prevents early lock-in to bad folder structures
- Avoids mixing narrative, evidence, and experimentation
- Makes later file-level decisions obvious instead of debatable
- Ensures the KnowledgeHub scales without becoming noisy

This phase is about *thinking once instead of fixing forever*.

---

## Phase 3 — Workflow & Governance Design

### Objective
Define a **pause-safe, drift-resistant workflow** for upgrading, maintaining, and extending the KnowledgeHub over time.

This phase answers:
- In what order do we work?
- How do we know when something is “done”?
- How do we stop and resume without re-alignment?
- How do decisions get recorded?

---

### Workflow Design Rules

- Every phase must have:
  - A clear entry condition
  - A clear exit condition
- No task larger than one focused session
- No phase overlaps in responsibility
- No silent assumptions

---

### Core Workflow Phases (High-Level)

- Planning & alignment
- Structural changes
- Content population
- Review & QA
- Deployment & validation

(Execution details come later; this phase defines the logic only.)

---

### Alignment & Recalibration Points

- Explicit Io–Ceven alignment checkpoints between phases
- Short written summaries of decisions taken
- Clear confirmation before moving to the next phase

This avoids invisible drift.

---

### Task & Change Tracking Philosophy

- Changes are logged, not just committed
- Rationale matters as much as outcome
- Future-you must understand past-you without reverse engineering

Tool choice is deferred; principles come first.

---

### Outputs

- A documented phase-based workflow
- Defined milestone checkpoints
- Agreed rules for task granularity and scope
- A governance mindset that prioritizes clarity over speed

---

### Reasoning

- Makes a long project feel light and controllable
- Protects against burnout and over-engineering
- Enables confident pauses without loss of context
- Turns the KnowledgeHub into a maintainable system, not a one-off effort

This phase is what makes the project sustainable and even enjoyable.

---

## End of Planning Phases (1–3)

Note:
- No files are changed during these phases
- No content is written
- No aesthetics are discussed
- Execution begins only after explicit phase closure
