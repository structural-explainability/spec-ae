# Conformance Checklist

This document defines the criteria for determining whether an artifact
conforms to the Accountable Entities specification.

Identifiers referenced in this document are the sole normative reference.
Section ordering, formatting, and presentation are non-normative.

An artifact may be a specification, schema, implementation, repository,
or other deliverable claiming conformance.

## Conformance Overview

An artifact CONFORMS if and only if:

- all mandatory requirements are satisfied
- no prohibited assertions are present
- conformance with Structural Explainability (SE) is preserved

Failure of any single check constitutes non-conformance.

AE.CONFORMANCE.SE.REQUIRED

- [ ] The artifact explicitly claims conformance with Structural Explainability.
- [ ] No requirement weakens or contradicts SE neutrality constraints.
- Fail if: conformance is asserted without explicit SE conformance.

AE.DEFINITION.CORE

- [ ] The artifact treats entity kinds and identity regimes as structural constructs.
- [ ] The artifact limits scope to defining entity kinds and identity regimes only.
- Fail if: behavioral, interpretive, or evaluative semantics are introduced.

AE.EXTENSION.ADMISSIBILITY

- [ ] No new entity kinds are introduced within the current version.
- [ ] No extension mechanisms bypass explicit versioning.
- [ ] Any reference to future extension defers to explicit, versioned criteria.
- Fail if: extension is permitted without version increment and justification.

AE.EXTENSION.VERSIONED_ONLY

- [ ] Entity kind extension is not permitted within the current version.
- [ ] Version boundaries governing extension are explicit.
- Fail if: extension is allowed implicitly or informally.

AE.IDENTITY.REGIME.MAPPING

- [ ] Each entity kind maps to exactly one identity regime.
- [ ] Identity regimes are explicit and structurally defined.
- [ ] Identity regimes are distinct across kinds.
- Fail if: identity rules are shared, implicit, or interpretation-dependent.

AE.KIND.CLOSED_SET.V1

- [ ] A closed set of entity kinds is defined.
- [ ] Every accountable entity is classified into exactly one kind.
- Fail if: entities may belong to multiple kinds or to none.

AE.KIND.EXACT_COUNT.V1

- [ ] Exactly six entity kinds are defined.
- [ ] No additional kinds are referenced or implied.
- Fail if: the number of kinds differs from six.

AE.KIND.K1

- [ ] The first entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.KIND.K2

- [ ] The second entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.KIND.K3

- [ ] The third entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.KIND.K4

- [ ] The fourth entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.KIND.K5

- [ ] The fifth entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.KIND.K6

- [ ] The sixth entity kind is defined explicitly.
- [ ] Its identity regime is distinct from all other kinds.

AE.SCOPE.EXCLUSIONS

Verify that the artifact does not define:

- [ ] domain vocabularies
- [ ] behavioral models
- [ ] causal explanations
- [ ] epistemic evaluation
- [ ] normative judgment or enforcement
- [ ] exchange or interaction mechanisms

Presence of any of the above constitutes non-conformance.

## Final Determination

An artifact CONFORMS if:

- all checks above pass, and
- no prohibited assertions are present.

Otherwise, the artifact is NON-CONFORMANT.

## Conformance Declaration

Artifacts claiming conformance SHOULD include a declaration of the form:

```text
Conforms to: AE Specification vx.y
Conforms to: SE Specification vx.y
```
