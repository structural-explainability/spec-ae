# Accountable Entities Specification (AE)

Status: Normative

This document defines the normative requirements for conformance with
Accountable Entities (AE).

AE is a downstream specification that conforms to Structural Explainability (SE).
All SE neutrality constraints apply.

AE defines an accountability-facing structural projection of SE profile kinds.
AE does not define new identity regimes, persistence rules, transformation
semantics, interpretation, governance authority, or enforcement.

## How to Read This Spec

Keywords MUST, MUST NOT, SHOULD, and MAY
are to be interpreted as described in RFC 2119.

Use of terms such as "canonical" denotes structural role only and
does not imply epistemic, causal, or normative preference.

This specification does not prescribe editorial structure,
terminology preference, or documentation layout beyond identifier semantics.

## Representation vs Constraint Classes

Some requirements describe what accountable entity structures MAY represent,
while others constrain how such representations MUST NOT be interpreted.

Overlap between these classes is intentional:
representation permissions do not imply explanatory, epistemic,
causal, normative, authoritative, or enforcement commitment.

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
the Structural Explainability (SE) specification.

AE MUST NOT weaken, override, or reinterpret any SE neutrality constraints.

## AE.DEFINITION.CORE

Accountable Entities defines a closed accountability-facing set of entity kinds
that map to upstream SE profile kinds.

AE defines accountable entity kinds as structural classifications only.

AE does not define:

- new identity regimes
- new persistence rules
- new transformation semantics
- domain vocabularies
- interpretation semantics
- governance authority
- legitimacy
- obligation
- enforcement

Accountable entity kinds inherit identity-and-persistence behavior from their
corresponding upstream SE profile kinds.

## AE.EXTENSION.ADMISSIBILITY

Any extension to the accountable entity kind set in a future version MUST satisfy
all of the following criteria:

- conformance with Structural Explainability
- explicit mapping to upstream SE profile-kind structure
- demonstration that the new kind cannot be represented as a specialization,
  composition, or interpretation of an existing accountable entity kind
- neutrality with respect to epistemic, causal, normative, authoritative,
  legitimacy-bearing, obligation-bearing, and enforcement interpretation
- explicit versioning under a new major version of this specification

Failure to meet any criterion renders the extension inadmissible.

## AE.EXTENSION.VERSIONED_ONLY

Extension of the accountable entity kind set is permitted only in a new major
version of this specification.

No extension is permitted within AE v1.

## AE.IDENTITY.REGIME.MAPPING

Each accountable entity kind MUST map to exactly one upstream SE profile kind.

The upstream SE profile kind determines identity-and-persistence behavior.

AE MUST NOT redefine:

- identity regimes
- profile kinds
- persistence outcomes
- transformation behavior
- identity relevance
- identity preservation
- identity breakage

Mappings MUST be structurally explicit and interpretation-neutral.

## AE.KIND.CLOSED_SET.V1

The set of accountable entity kinds defined by AE v1 is closed.

All conforming systems MUST classify each accountable entity into exactly one
defined accountable entity kind.

No conforming system MAY classify one accountable entity into multiple AE kinds
or into no AE kind.

## AE.KIND.EXACT_COUNT.V1

AE v1 defines exactly nine accountable entity kinds.

No additional accountable entity kinds are permitted for conformance.

The nine accountable entity kinds correspond to the nine upstream SE profile
kinds used by AE v1.

## AE.KIND.PER.CTX_E

The `AE.KIND.PER.CTX_E` accountable entity kind is defined explicitly.

It maps exactly to the upstream `CTX_E` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.CTX_S

The `AE.KIND.PER.CTX_S` accountable entity kind is defined explicitly.

It maps exactly to the upstream `CTX_S` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.ENR_I

The `AE.KIND.PER.ENR_I` accountable entity kind is defined explicitly.

It maps exactly to the upstream `ENR_I` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.ENR_L

The `AE.KIND.PER.ENR_L` accountable entity kind is defined explicitly.

It maps exactly to the upstream `ENR_L` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.NOR_C

The `AE.KIND.PER.NOR_C` accountable entity kind is defined explicitly.

It maps exactly to the upstream `NOR_C` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.NOR_S

The `AE.KIND.PER.NOR_S` accountable entity kind is defined explicitly.

It maps exactly to the upstream `NOR_S` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.OBL

The `AE.KIND.PER.OBL` accountable entity kind is defined explicitly.

It maps exactly to the upstream `OBL` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.OCC

The `AE.KIND.PER.OCC` accountable entity kind is defined explicitly.

It maps exactly to the upstream `OCC` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.KIND.PER.REC

The `AE.KIND.PER.REC` accountable entity kind is defined explicitly.

It maps exactly to the upstream `REC` profile kind.

The identifier is structural. It MUST NOT be interpreted as defining domain
meaning, epistemic authority, legal status, social role, or enforcement effect.

## AE.SCOPE.EXCLUSIONS

This specification does not define:

- domain vocabularies
- behavioral models
- causal explanations
- epistemic evaluation
- authority
- legitimacy
- obligation
- normative judgment or enforcement
- exchange or interaction mechanisms
- governance, approval, or lifecycle rules
- contextual evidence, explanation, or attestation interfaces
- new identity regimes
- new persistence rules
- new transformation semantics

These concerns are explicitly out of scope.
