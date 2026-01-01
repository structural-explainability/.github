# Structural Explainability

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/.github/actions/workflows/ci.yml/badge.svg)
[![Check Links](https://github.com/structural-explainability/.github/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/.github/actions/workflows/links.yml)

> Defines neutral constraints under which explainability is possible without embedding interpretation.

Structural Explainability defines the minimal, stable constraints
under which identity, structure, change, explanation, and persistent disagreement
can coexist over time without embedding interpretation.

It characterizes the representational conditions required for explainability
to remain possible across incompatible
legal, political, scientific, or normative frameworks.

This organization contains specifications, formalizations, and papers
that define, justify, and defend that neutral space.

## Roles

This organization is structured around roles:

| Role                                                              | Purpose                                                             |
| ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| [**Specifications**](#normative-specifications)                   | Define what must be true for admissibility                          |
| [**Formalizations**](#formalizations)                             | Demonstrate that specifications are internally consistent           |
| [**Foundations**](#foundations)                                   | Establish the underlying theoretical results                        |
| [**Papers**](#papers)                                             | Justify why the constraints are necessary and unavoidable           |
| [**Boundaries & Overlays**](#boundary-and-overlay-specifications) | Define how interpretation may attach without entering the substrate |

## Specifications (Normative)

These repositories define the admissible representational space
for structurally explainable systems.
They are normative only in the sense of **defining structural constraints**, not interpretations.

### Structural Explainability (Foundation)

Defines neutrality and boundary constraints that apply to all downstream systems.

| Repository                                                      | Purpose                                                        | Status    |
| --------------------------------------------------------------- | -------------------------------------------------------------- | --------- |
| [spec-se](https://github.com/structural-explainability/spec-se) | Neutrality and boundary constraints for all downstream systems | Normative |

### Neutral Substrate (AE / EP)

These repositories define the core representational substrate
for structurally explainable systems.

| Repository                                                      | Purpose                                   | Status    |
| --------------------------------------------------------------- | ----------------------------------------- | --------- |
| [spec-ae](https://github.com/structural-explainability/spec-ae) | Accountable Entities and identity regimes | Normative |
| [spec-ep](https://github.com/structural-explainability/spec-ep) | Graph evolution over accountable entities | Normative |

### Interface (CEE)

The Contextual Evidence and Explanation (CEE) layer defines
a structural interface to the neutral substrate.
It does not alter identity, structure, or recorded change.

| Repository                                                        | Purpose                                                       | Status    |
| ----------------------------------------------------------------- | ------------------------------------------------------------- | --------- |
| [spec-cee](https://github.com/structural-explainability/spec-cee) | Contextual evidence, explanation, attestation, and provenance | Normative |

### Boundaries (GB / IB)

These repositories define additional structural boundaries
that operate relative to the neutral substrate.
They do not alter identity, structure, or recorded change.
They serve as guardrails that prevent interpretation from leaking into the neutral substrate.

| Repository                                                        | Purpose                                                       | Status    |
| ----------------------------------------------------------------- | ------------------------------------------------------------- | --------- |
| [spec-gb](https://github.com/structural-explainability/spec-gb)   | Governance boundary for structural artifacts and actions      | Normative |
| [spec-ib](https://github.com/structural-explainability/spec-ib)   | Interpretation boundary for external frameworks               | Normative |

### Informative

| Repository                                                                        | Purpose                                             | Status      |
| --------------------------------------------------------------------------------- | --------------------------------------------------- | ----------- |
| [spec-se-appendix](https://github.com/structural-explainability/spec-se-appendix) | Identifier rules, examples, and cross-spec patterns | Informative |

## Formalizations

These repositories **do not define meaning or behavior**.
They demonstrate that the specifications are internally consistent,
coherent, and composable under formal reasoning.

### Structural Explainability (Foundation)

Structural Explainability formalizes the **minimal, stable constraints**
under which identity, structure, change, explanation, and persistent disagreement
can coexist over time without embedding interpretation,
and establishes why those constraints are necessary.

| Repository                                                                                        | Purpose                     | CI                                                                                                                          | Description                           |
| ------------------------------------------------------------------------------------------------- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| [StructuralExplainability](https://github.com/structural-explainability/StructuralExplainability) | Cross-cutting constraints   | ![CI](https://github.com/structural-explainability/StructuralExplainability/actions/workflows/ci.yml/badge.svg?branch=main) | Neutrality and conformance predicates |
| [NeutralSubstrate](https://github.com/structural-explainability/NeutralSubstrate) | Neutrality theorem | ![CI](https://github.com/structural-explainability/NeutralSubstrate/actions/workflows/ci.yml/badge.svg?branch=main) | Substrates stable under incompatible extensions must be pre-causal and pre-normative                                                  |
| [IdentityRegimes](https://github.com/structural-explainability/IdentityRegimes)   | Identity regimes   | ![CI](https://github.com/structural-explainability/IdentityRegimes/actions/workflows/ci.yml/badge.svg?branch=main)  | Six identity-and-persistence regimes are necessary and sufficient for accountability-oriented substrates under neutrality assumptions |

### Neutral Substrate (AE / EP)

These repositories formalize the neutral substrate defined by AE and EP.

| Repository                                                                                        | Purpose                     | CI                                                                                                                          | Description                           |
| ------------------------------------------------------------------------------------------------- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| [AccountableEntities](https://github.com/structural-explainability/AccountableEntities)           | Entity-regime instantiation | ![CI](https://github.com/structural-explainability/AccountableEntities/actions/workflows/ci.yml/badge.svg?branch=main)      | Formalization of AE identity regimes  |
| [EvolutionProtocol](https://github.com/structural-explainability/EvolutionProtocol)               | Neutral exchange substrate  | ![CI](https://github.com/structural-explainability/EvolutionProtocol/actions/workflows/ci.yml/badge.svg?branch=main)        | Formalization of EP graph evolution   |

### Interface (CEE)

This repository formalizes **the structural interface layer**
over the neutral substrate.

| Repository                                                                                    | Purpose                 | CI                                                                                                                        | Description                                                                |
| --------------------------------------------------------------------------------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| [CEE](https://github.com/structural-explainability/CEE)                                       | Explanation overlay     | ![CI](https://github.com/structural-explainability/CEE/actions/workflows/ci.yml/badge.svg?branch=main)                    | Structural forms for contextual explanation and evidence                   |


### Boundaries (GB / IB)

These repositories formalize **additional structural boundaries**
that operate relative to the neutral substrate.
They keep interpretation from leaking into the neutral substrate.

| Repository                                                                                    | Purpose                 | CI                                                                                                                        | Description                                                                |
| --------------------------------------------------------------------------------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| [GovernanceBoundary](https://github.com/structural-explainability/GovernanceBoundary)         | Governance boundary     | ![CI](https://github.com/structural-explainability/GovernanceBoundary/actions/workflows/ci.yml/badge.svg?branch=main)     | Governance                                                                 |
| [InterpretationBoundary](https://github.com/structural-explainability/InterpretationBoundary) | Interpretation boundary | ![CI](https://github.com/structural-explainability/InterpretationBoundary/actions/workflows/ci.yml/badge.svg?branch=main) | Conditions under which external frameworks may interpret substrate records |


## Papers

Papers provide theoretical justification for foundational specifications.
They are explanatory, not normative.

| Repository                                                                                              | Focus              | Status    | Description                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------- | ------------------ | --------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate) | Neutrality theorem | Submitted | Narrative exposition of the neutrality theorem and its formal proof, establishing design constraints for neutral representational substrates |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes)   | Identity regimes   | Submitted | Narrative exposition of the identity-regimes result and its formal justification                                                             |


## Design Commitments

Across all repositories:

- Identity precedes explanation.
- Structure and change are recorded without interpretation.
- Interpretation remains external, attributable, and contestable.
- Disagreement is representable and not forced to resolve.
- No domain semantics are embedded in the core.

## Intentionally Excluded

The following are intentionally excluded from this organization:

- Domain vocabularies (except clearly labeled examples)
- Application schemas or data models
- Analytics, inference, or decision systems
- Governance or enforcement frameworks
- Visualization or tooling layers

Domain projects may claim conformance with these specifications, but are outside this core.

## How to Use This Organization

- **To implement Structural Explainability**, start with the specifications.
- **To understand the justification**, start with the papers.
- **To verify coherence**, consult the Lean formalizations.

## Core Statement

Structural Explainability defines a neutral structural substrate
that enables explainability by preserving identity, structure, and change
while allowing disagreement to remain external, attributable, and unresolved.

At its core, Structural Explainability is concerned with identity.
Stable identity is the precondition for explanation, provenance, and disagreement over time.
Identity must persist independently of interpretation, authority, or consensus.

Structural Explainability defines the complete admissible space of representation.
It simultaneously bounds what representation must not do and
contains all representation that is permitted.
Within this space, identity, structure, and change may be recorded,
while interpretation, explanation, and judgment are constrained
to remain external to the substrate.

- **Accountable Entities** define identity regimes
  that allow entities to persist across time and change.
- **Evolution Protocol** defines the evolution of structural relationships among those entities,
  recording change without embedding explanation.

Together, they form the structural substrate.

- **Contextual Evidence & Explanations** provide the structural interface
  by which external interpretation may be attached to, referenced from, and reasoned about,
  without entering or contaminating the substrate.
- Context tags, explanations, attestations, and provenance are not facts about the world;
  they are structured references to interpretive acts that occur outside the substrate.

Interpretation does not disappear.
It is made explicit, attributable, and contestable.

Structural Explainability is not anti-interpretation;
it is anti-implicit interpretation.
Elements of interpretation may exist only in forms
that do not alter identity, structure, or recorded change.

Structural Explainability is designed for plural systems:
independent implementations that represent the same phenomena in different ways.
Uniform naming, shared ontologies, or centralized authority are not required.
Differences are addressed through explicit, accountable mappings
rather than forced normalization or consensus.

Domains such as science, model development, and law do not alter the substrate.
They specialize explanation by contributing controlled vocabularies for contextual scoping.
These vocabularies are constrained by Structural Explainability and
do not assert truth, causality, or normativity.

The result is a system that records reality without deciding its meaning,
enables explanation without enforcing agreement, and
supports long-term coordination across disagreement, institutional change, and time.
