# Accountable Entities Identifiers (AE)

This document defines the stable requirement identifiers used by the
Accountable Entities (AE) specification.

Identifiers are the sole normative reference mechanism.
Section ordering, formatting, and presentation are non-normative.

## Overview

Defines the admissible entity kinds and identity-and-persistence regimes
under the neutrality constraints of Structural Explainability (SE).

## Identifier Semantics and Ordering

Identifiers are the sole normative reference mechanism.
Section ordering, formatting, and presentation are non-normative.

Identifiers are listed in strict alphabetical order to remove
editorial discretion and ensure deterministic placement.

## Identifier Naming Rules

All identifiers follow this pattern:

All identifiers begin with `AE.` and use uppercase dot-separated semantic terms.

Identifiers are:

- semantic, not positional
- stable across versions
- reusable across prose, code, and formal proofs
- language-agnostic
- suitable for direct mapping to Lean theorem names

Identifiers MUST NOT be renamed or repurposed.
New identifiers MAY be added only in a new major version of this document.

## Identifier Notes

Each identifier MUST be followed by exactly one note.

- The note MUST be expressed as a single bullet.
- The bullet text MAY wrap across lines.
- No additional bullets, sublists, or structural markers are permitted.
- Notes are explanatory only and do not introduce additional requirements.

## Canonical Identifier List (Alphabetical, with Notes)

AE.CONFORMANCE.SE.REQUIRED

- States that Accountable Entities conforms to the Structural Explainability specification.

AE.DEFINITION.CORE

- Defines Accountable Entities as a structural specification for entity kinds and identity regimes.

AE.EXTENSION.ADMISSIBILITY

- Defines the criteria that any future extension of the entity kind set MUST satisfy.

AE.EXTENSION.VERSIONED_ONLY

- States that extension of entity kinds is permitted only in a new major version of the specification.

AE.IDENTITY.REGIME.MAPPING

- Requires that each entity kind corresponds to a distinct identity and persistence regime.

AE.KIND.CLOSED_SET.V1

- States that the set of accountable entity kinds is closed for AE v1.

AE.KIND.EXACT_COUNT.V1

- States that exactly six accountable entity kinds are defined for AE v1.

AE.KIND.PER.CTX_E

- Placeholder for the Person entity kind under the Contextual-Epistemic regime.

AE.KIND.PER.CTX_S

- Placeholder for the Person entity kind under the Contextual-Social regime.

AE.KIND.PER.ENR_I

- Placeholder for the Person entity kind under the Enactment-Instrumental regime.

AE.KIND.PER.ENR_L

- Placeholder for the Person entity kind under the Enactment-Legal regime.

AE.KIND.PER.NOR_C

- Placeholder for the Person entity kind under the Normative-Contractual regime.

AE.KIND.PER.NOR_S

- Placeholder for the Person entity kind under the Normative-Social regime.

AE.KIND.PER.OBL

- Placeholder for the Person entity kind under the Obligatory regime.

AE.KIND.PER.OCC

- Placeholder for the Person entity kind under the Occurrent regime.

AE.KIND.PER.REC

- Placeholder for the Person entity kind under the Record regime.

AE.SCOPE.EXCLUSIONS

- Defines what Accountable Entities explicitly does not specify.

## Cross-Artifact Consistency Rule

Each identifier in this list MUST appear:

- exactly once in SPEC.md
- exactly once in CONFORMANCE.md
- exactly once as a field in the Lean `ConformanceEvidence` structure
- exactly once in the Lean requirements list

Alphabetical order SHOULD be preserved across all artifacts.
