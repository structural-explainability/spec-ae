# Conformance Checklist

This document defines the criteria for determining whether an artifact
conforms to the Accountable Entities (AE) specification.

Identifiers referenced in this document are the sole normative reference.
Section ordering, formatting, and presentation are non-normative.

An artifact may be a specification, schema, implementation, repository,
or other deliverable claiming conformance.

## Conformance Overview

An artifact CONFORMS if and only if:

- all mandatory requirements are satisfied
- no prohibited assertions are present
- conformance with Structural Explainability (SE) is preserved
- conformance with the upstream SE profile-kind contract is preserved

Failure of any single check constitutes non-conformance.

## AE.CONFORMANCE.SE.REQUIRED

- [ ] The artifact explicitly claims conformance with Structural Explainability.
- [ ] No requirement weakens, overrides, or contradicts SE neutrality constraints.
- Fail if: AE conformance is asserted without explicit SE conformance.

## AE.DEFINITION.CORE

- [ ] The artifact treats accountable entity kinds as structural classifications.
- [ ] The artifact treats accountable entity kinds as an accountability-facing
- projection of upstream SE profile kinds.
- [ ] The artifact limits scope to defining accountable entity kinds and their
- required mappings to SE profile kinds.
- Fail if: behavioral, causal, interpretive, epistemic, evaluative, authoritative,
  legitimacy-bearing, obligation-bearing, or enforcement semantics are introduced.

## AE.EXTENSION.ADMISSIBILITY

- [ ] No new accountable entity kinds are introduced within the current version.
- [ ] No extension mechanisms bypass explicit versioning.
- [ ] Any reference to future extension defers to explicit, versioned criteria.
- Fail if: extension is permitted without version increment and justification.

## AE.EXTENSION.VERSIONED_ONLY

- [ ] Accountable entity kind extension is not permitted within the current version.
- [ ] Version boundaries governing extension are explicit.
- Fail if: extension is allowed implicitly or informally.

## AE.IDENTITY.REGIME.MAPPING

- [ ] Each accountable entity kind maps to exactly one upstream SE profile kind.
- [ ] Each upstream SE profile kind is explicit and structurally defined upstream.
- [ ] AE does not redefine profile identity, persistence, or transformation behavior.
- Fail if: profile mappings are shared ambiguously, implicit, missing, duplicated, or interpretation-dependent.

## AE.KIND.CLOSED_SET.V1

- [ ] A closed set of accountable entity kinds is defined.
- [ ] Every accountable entity is classified into exactly one accountable entity kind.
- Fail if: accountable entities may belong to multiple AE kinds or to none.

## AE.KIND.EXACT_COUNT.V1

- [ ] Exactly nine accountable entity kinds are defined.
- [ ] No additional accountable entity kinds are referenced or implied.
- Fail if: the number of accountable entity kinds differs from nine.

## AE.KIND.PER.CTX_E

- [ ] The `AE.KIND.PER.CTX_E` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `CTX_E` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.CTX_E` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `CTX_E`.

## AE.KIND.PER.CTX_S

- [ ] The `AE.KIND.PER.CTX_S` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `CTX_S` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.CTX_S` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `CTX_S`.

## AE.KIND.PER.ENR_I

- [ ] The `AE.KIND.PER.ENR_I` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `ENR_I` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.ENR_I` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `ENR_I`.

## AE.KIND.PER.ENR_L

- [ ] The `AE.KIND.PER.ENR_L` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `ENR_L` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.ENR_L` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `ENR_L`.

## AE.KIND.PER.NOR_C

- [ ] The `AE.KIND.PER.NOR_C` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `NOR_C` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.NOR_C` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `NOR_C`.

## AE.KIND.PER.NOR_S

- [ ] The `AE.KIND.PER.NOR_S` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `NOR_S` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.NOR_S` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `NOR_S`.

## AE.KIND.PER.OBL

- [ ] The `AE.KIND.PER.OBL` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `OBL` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.OBL` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `OBL`.

## AE.KIND.PER.OCC

- [ ] The `AE.KIND.PER.OCC` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `OCC` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.OCC` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `OCC`.

## AE.KIND.PER.REC

- [ ] The `AE.KIND.PER.REC` accountable entity kind is defined explicitly.
- [ ] It maps exactly to the upstream `REC` profile kind.
- [ ] It is not renamed, merged, split, or reinterpreted.
- Fail if: `AE.KIND.PER.REC` is missing, renamed, merged, split,
  reinterpreted, or mapped to any profile kind other than `REC`.

## AE.SCOPE.EXCLUSIONS

Verify that the artifact does not define:

- [ ] domain vocabularies
- [ ] behavioral models
- [ ] causal explanations
- [ ] epistemic evaluation
- [ ] authority
- [ ] legitimacy
- [ ] obligation
- [ ] normative judgment or enforcement
- [ ] exchange or interaction mechanisms
- [ ] governance, approval, or lifecycle rules
- [ ] contextual evidence, explanation, or attestation interfaces
- [ ] new identity regimes
- [ ] new persistence rules
- [ ] new transformation semantics

Presence of any excluded concern as an AE-defined construct constitutes non-conformance.

## Final Determination

An artifact CONFORMS if:

- all checks above pass
- no prohibited assertions are present
- conformance with Structural Explainability is preserved
- conformance with the upstream SE profile-kind contract is preserved

Otherwise, the artifact is NON-CONFORMANT.

## Conformance Declaration

Artifacts claiming conformance SHOULD include a declaration of the form:

```text
Conforms to: AE Specification vX.Y
Conforms to: SE Specification vX.Y
Conforms to: SE Profile Kind Contract vX.Y
```
