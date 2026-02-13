```yaml
id: GOV-ADR-01
layer: governance
type: decision record
phase: X
status: frozen
created: 2026-02-10
updated: 2026-02-13
```
# ADR | Metadata Schema v0.2

## Context

During Phase 4 architectural redesign, it became clear that the original minimal YAML schema (`title, type, domain, status`) was sufficient for navigation but insufficient for:

- Traceability
- Cross-linking
- Governance signaling
- Professional portfolio positioning
- Evidence mapping

A controlled expansion was required.

---

## Decision

Adopt **Metadata Schema v0.2**, consisting of:

### Required Fields (Global)

- `title`
- `type`
- `domain`
- `status`

These remain mandatory for all pages.

---

### Global Optional Fields

- `id`
- `summary`
- `tags`
- `created`
- `updated`
- `maturity`
- `evidence`
- `related`

These enhance traceability and professional clarity without introducing structural complexity.

---

### Domain-Specific Extensions

#### Prompt Engineering
- `models`
- `eval_axes`
- `metrics`
- `artifacts`
- `claims`

#### Workflows
- `workflow_steps`
- `inputs`
- `outputs`
- `failure_modes`
- `recovery`
- `routing_policy_ref`

#### Documentation / ADR
- `adr_id`
- `decision`
- `context`
- `consequences`
- `policy_scope`

---

## Explicit Non-Goals

- No audience field (removed intentionally).
- No heavy taxonomy layers.
- No nested metadata objects.
- No automated validation layer at this stage.

---

## Rationale

This schema balances:

- Professional rigor
- Governance clarity
- Scalability
- Authoring simplicity

It strengthens the KnowledgeHub’s architectural credibility while avoiding overengineering.

---

## Status

Canonical as of Phase 4 redesign.
Future revisions require new ADR.
