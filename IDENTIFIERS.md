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

AE.<CATEGORY>.<SUBCATEGORY>.<QUALIFIER>

Identifiers are:

- semantic, not positional
- stable across versions
- reusable across prose, code, and formal proofs
- language-agnostic
- suitable for direct mapping to Lean theorem names

Identifiers MUST NOT be renamed or repurposed.
New identifiers MAY be added only in a new major version of AE.

## Canonical Identifier List (Alphabetical, with Notes)

AE.CONFORMANCE.SE.REQUIRED
States that Accountable Entities conforms to the Structural Explainability specification.

AE.DEFINITION.CORE
Defines Accountable Entities as a structural specification for entity kinds and identity regimes.

AE.EXTENSION.ADMISSIBILITY
Defines the criteria that any future extension of the entity kind set MUST satisfy.

AE.EXTENSION.VERSIONED_ONLY
States that extension of entity kinds is permitted only in a new major version of the specification.

AE.IDENTITY.REGIME.MAPPING
Requires that each entity kind corresponds to a distinct identity and persistence regime.

AE.KIND.CLOSED_SET.V1
States that the set of accountable entity kinds is closed for AE v1.

AE.KIND.EXACT_COUNT.V1
States that exactly six accountable entity kinds are defined for AE v1.

AE.KIND.K1
Placeholder for the first accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.KIND.K2
Placeholder for the second accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.KIND.K3
Placeholder for the third accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.KIND.K4
Placeholder for the fourth accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.KIND.K5
Placeholder for the fifth accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.KIND.K6
Placeholder for the sixth accountable entity kind defined in AE v1.
Specific semantics are defined in SPEC.md.

AE.SCOPE.EXCLUSIONS
Defines what Accountable Entities explicitly does not specify.

## Cross-Artifact Consistency Rule

Each identifier in this list MUST appear:

- exactly once in SPEC.md
- exactly once in CONFORMANCE.md
- exactly once as a field in the Lean ConformanceEvidence structure
- exactly once in the Lean requirements list

Alphabetical order SHOULD be preserved across all artifacts.
