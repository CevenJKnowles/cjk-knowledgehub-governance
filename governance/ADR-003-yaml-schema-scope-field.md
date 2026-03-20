---
id: ADR-003
title: "ADR | YAML Schema Extension — scope Field"
type: adr
status: active
version: "1.0"
created: 2026-03-20
updated: 2026-03-20
provenance: human
scope: [knowledgehub]
tags: [governance, schema, yaml, tpl-001]
related: [TPL-001]
ref: []
repo: []
---

# ADR | YAML Schema Extension — scope Field

---

## Context

TPL-001 defines the canonical YAML header schema for all documents in the CJK governance ecosystem. As work across multiple distinct projects (IO-III Architecture, KnowledgeHub, Prompt Pattern Library) accelerates, ADRs and governance documents require an explicit, machine-readable field that declares which project a document governs.

Without this field, scope is inferred from folder location or tags alone, which is insufficient for cross-repo traceability and professional review.

---

## Decision

Add a `scope` field to the TPL-001 YAML header schema.

- Field name: `scope`
- Type: controlled lowercase list
- Position: after `provenance`, before `tags`
- Required: no (optional for documents with obvious single-project scope; recommended for all new documents)

```yaml
scope: [knowledgehub]
```

Multi-scope example where a decision genuinely crosses projects:

```yaml
scope: [knowledgehub, prompt-pattern-library]
```

---

## Alternatives Considered

**Use `tags` only** — rejected. Tags are informal and non-authoritative. A governance field requires a dedicated, structured key that is unambiguous and queryable.

**Use `repo` field** — rejected. `repo` records external repository *references*, not the project a document *governs*. These are distinct concepts and must remain separate fields.

**Encode scope in filename prefix** — rejected. TPL-001 settled on 2-tier `{TYPE}-{SEQ}-[slug].md` specifically to avoid encoding structural metadata in filenames. Reversing that decision for scope alone would be inconsistent.

---

## Rationale

`scope` is the minimal addition that makes project governance unambiguous. It does not overlap with any existing field. It is consistent with the TPL-001 philosophy of explicit, structured metadata over inferred context. A controlled list allows single and multi-project scope to be expressed cleanly.

---

## Non-Goals / Constraints

- This field does not replace `tags`, `related`, `ref`, or `repo`.
- It does not introduce a validation layer — no automated enforcement at this stage, consistent with GOV-ADR-01.
- It does not retroactively apply to existing documents. TPL-001 transition rules apply.
- Controlled vocabulary is not formally defined beyond lowercase project identifiers. No registry is created at this stage.

---

## Consequences

- All new KnowledgeHub ADRs carry `scope: [knowledgehub]`.
- TPL-001 should be updated to document this field at next revision (MAJOR increment to v2.0).
- Cross-project ADRs are now expressible without ambiguity.

---

## Supersedes

None.

---

## Review Trigger

Revisit if a formal multi-repo governance layer is introduced, or if automated schema validation is added.
