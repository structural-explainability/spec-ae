# Accountable Entities Specification (AE)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Build Status](https://github.com/structural-explainability/spec-ae/actions/workflows/ci.yml/badge.svg)
[![Check Links](https://github.com/structural-explainability/spec-ae/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/spec-ae/actions/workflows/links.yml)

> Authoritative specification of Accountable Entities (AE).

## Overview

The Accountable Entities (AE) specification defines the structural requirements
for representing entities whose identity and persistence must remain explicit,
traceable, and stable under reinterpretation.

AE is defined as a downstream specification that conforms to Structural Explainability (SE).
It introduces no epistemic, causal, or normative
commitments beyond those permitted by SE.

## Purpose

The purpose of AE is to specify
**what kinds of entities must be representable**
in order for accountability, traceability, and
persistence over time to be structurally possible.

AE concerns entity kinds and identity regimes only. It does not define behavior,
interpretation, explanation, or evaluation.

## Versioning and Closure

AE v1 defines a **closed set of entity kinds** for the purpose of conformance.

For AE v1:

- exactly six entity kinds are defined
- no additional kinds are permitted for conformance
- all conforming systems MUST classify accountable entities into one of the
  defined kinds

Closure applies only to AE v1 and does not assert metaphysical finality.

## Extension Policy

Extension of the entity kind set is explicitly permitted only under a new
version of the specification.

Any future extension MUST:

- preserve conformance with Structural Explainability
- introduce explicit identity and persistence rules for the new kind
- demonstrate that the new kind cannot be represented as a specialization or
  composition of existing kinds
- remain neutral with respect to epistemic, causal, and normative interpretation

Extension is expected to be rare and requires explicit justification.

## Scope

This specification defines:

- the existence of accountable entity kinds
- the requirement that each kind corresponds to a distinct identity regime
- the closure and extension rules governing the kind set

This specification does NOT define:

- domain vocabularies
- application-specific semantics
- behavioral models
- explanation mechanisms
- evaluation or enforcement logic

## Relationship to Other Work

- AE **conforms to** the Structural Explainability Specification.
- AE provides entity foundations for downstream specifications such as exchange
  protocols and contextual explanations.
- Application domains that interpret or evaluate entities are out of scope.

## Repository Contents

- [SPEC.md](./SPEC.md) - Normative specification
- [IDENTIFIERS.md](./IDENTIFIERS.md) - Stable requirement identifiers
- [CONFORMANCE.md](./CONFORMANCE.md) - Conformance checklist
- [ANNOTATIONS.md](./ANNOTATIONS.md) - Annotation standards
- [LICENSE](./LICENSE) - licensing terms
- [CITATION.cff](./CITATION.cff) - Citation metadata
- [CHANGELOG.md](./CHANGELOG.md) - Version history

## Clarifying Statement

Accountable Entities define structural identity regimes, not domain semantics.

An entity kind in AE specifies how identity and persistence must be represented
in order to support accountability under change.
It does not assert what an entity is, what it does, or how it should be interpreted.

AE makes identity explicit so that structure can remain stable
across reinterpretation, disagreement, and changing explanatory frameworks.
