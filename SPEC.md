# Accountable Entities Specification (AE)

Status: Normative

This document defines the normative requirements for conformance with
Accountable Entities (AE).

AE is a downstream specification that conforms to Structural Explainability (SE).
All SE neutrality constraints apply.

## How to Read This Spec

Keywords MUST, MUST NOT, SHOULD, and MAY
are to be interpreted as described in RFC 2119.

Use of terms such as "canonical" denotes structural role only and
does not imply epistemic, causal, or normative preference.

This specification does not prescribe editorial structure,
terminology preference, or documentation layout beyond identifier semantics.

## Representation vs Constraint Classes

Some requirements describe what the substrate MAY represent,
while others constrain how such representations MUST NOT be interpreted.

Overlap between these classes is intentional:
representation permissions do not imply explanatory commitment.

## Identifier Semantics and Stability

Each requirement in this document is identified by a stable identifier
of the form `AE.*`.

Identifiers are the sole normative reference for conformance.
Textual wording MAY be clarified over time without changing meaning;
any change that alters the requirement MUST result in a new identifier.

Renaming, reordering, or relocating identifiers constitutes a semantic
change and is therefore intentionally diff-visible.

Repository paths, filenames, and section ordering are non-normative and
do not affect identifier meaning.

---

## AE.CONFORMANCE.SE.REQUIRED

Any system claiming conformance with this specification MUST also conform to
the Structural Explainability Specification.

AE MUST NOT weaken or override any SE neutrality constraints.

## AE.DEFINITION.CORE

Accountable Entities define a closed set of entity kinds whose identity and
persistence must be represented explicitly in order to support accountability,
traceability, and stability under reinterpretation.

AE specifies entity kinds and identity regimes only.

## AE.EXTENSION.ADMISSIBILITY

Any extension to the entity kind set in a future version MUST satisfy all of the
following criteria:

- conformance with Structural Explainability
- explicit definition of identity and persistence rules
- demonstration that the new kind cannot be represented as a specialization,
  composition, or interpretation of an existing kind
- neutrality with respect to epistemic, causal, and normative interpretation

Failure to meet any criterion renders the extension inadmissible.

## AE.EXTENSION.VERSIONED_ONLY

Extension of the entity kind set is permitted only in a new major version of this specification.

No extension is permitted within AE v1.

## AE.IDENTITY.REGIME.MAPPING

Each accountable entity kind MUST correspond to a distinct identity and
persistence regime.

The identity regime for a kind determines:

- how identity is established
- how identity persists over time
- how identity relates to change

Identity regimes MUST be structurally explicit and interpretation-neutral.

## AE.KIND.CLOSED_SET.V1

The set of accountable entity kinds defined by AE v1 is closed.

All conforming systems MUST classify accountable entities into exactly one of the
defined kinds.

## AE.KIND.EXACT_COUNT.V1

AE v1 defines exactly six accountable entity kinds.

No additional kinds are permitted for conformance.

## AE.KIND.K1

The first accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.KIND.K2

The second accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.KIND.K3

The third accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.KIND.K4

The fourth accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.KIND.K5

The fifth accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.KIND.K6

The sixth accountable entity kind defined by AE v1.

The identity regime for this kind MUST be defined explicitly and MUST be distinct
from the regimes of all other kinds.

## AE.SCOPE.EXCLUSIONS

This does not define:

- domain vocabularies
- behavioral models
- causal explanations
- epistemic evaluation
- normative judgment or enforcement
- exchange or interaction mechanisms

These concerns are explicitly out of scope.

