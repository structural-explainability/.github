# Structural Explainability

<!-- markdownlint-disable MD024 -->

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/.github/actions/workflows/ci-hygiene.yml/badge.svg?branch=main)
[![Check Links](https://github.com/structural-explainability/.github/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/.github/actions/workflows/links.yml)

> A research program on how records stay the same,
> or stop being the same, as they change,
> built on a foundation that
> makes no causal or normative claims of its own.

## Overview

Structural Explainability (SE) is a research program on how a record stays the
same thing, or stops being it, as it changes:
forks, revisions, merges, replications,
a body of law like 40 CFR whose parts change while the whole persists.
People mostly agree on these verdicts in practice.
The aim is to find out how they decide,
and to write the rules down explicitly enough that
two defensible rules can be compared and
their disagreement traced to specific commitments,
instead of being buried in an identifier.

The foundation is a neutral substrate,
designed to be pre-causal and pre-normative.
It makes no causal or normative claims of its own;
such claims can enter only as attributed assertions with a source.
Parties who disagree can still share the same records when the stated assumptions hold.
This foundation is formalized in Lean under stated assumptions.

What is open is which kinds of things need distinct identity treatment,
and why they must differ.
That remains active research.
Papers, specifications, and other repositories
written before this work may use an older inventory of
kinds and are being revised as the theory settles.

## Core Statement

SE keeps structural commitments separate from the claims built on them.
The foundation records identity, structure, transformation, and change;
interpretive claims sit above it, each attributed to a source.

Structural Explainability is not anti-interpretation;
it is anti-implicit interpretation.
Interpretation is welcome when it is stated, attributed, and open to dispute,
so disagreement remains explicit, attributable, and contestable over time.

SE supports independently developed accounts of identity and change
without requiring a single authority, ontology, or interpretation.

## Foundational and Related Theory

Lean 4 formalizations of SE concepts, relationships, and mathematical results.

Each repository owns its definitions, scientific claims, evidence,
implementation, documentation, and release information.

### Mathlib Mini (MM)

[Mathlib Mini](https://github.com/mathlib-mini/mathlib-mini) is a small,
unofficial, Mathlib-inspired foundation for Lean 4.

It provides the limited mathematical primitives needed by Structural
Explainability theory repositories without requiring the full Mathlib library.

Mathlib Mini depends only on Lean core.
Compatibility with corresponding Mathlib definitions and operations is verified separately.

- **Repository:** [mathlib-mini/mathlib-mini](https://github.com/mathlib-mini/mathlib-mini)
- **Documentation:** [Mathlib Mini](https://mathlib-mini.github.io/mathlib-mini/)

### Independent Theories

Independent (leaf) theories require no other SE theory repository.
Deps indicates a direct dependency on MM=MathlibMini or "-" for none.

| Deps | Repository                                                                                                          | Role in Structural Explainability                                                                                                                  |
| ---- | ------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| MM   | [se-theory-neutral-substrate](https://github.com/structural-explainability/se-theory-neutral-substrate)             | Neutral structural and referential foundations, admissibility, and interpretive boundaries.                                                        |
| MM   | [se-theory-persistence](https://github.com/structural-explainability/se-theory-persistence)                         | Identity survival and breakage under change, and the commitment calculus (consistency, required, forbidden, undetermined) other theories build on. |
| -    | [se-theory-transformation](https://github.com/structural-explainability/se-theory-transformation)                   | Structural transformation vocabulary, operators, and intrinsic change semantics.                                                                   |
| MM   | [se-theory-structural-assurability](https://github.com/structural-explainability/se-theory-structural-assurability) | Claim-relative evidentiary capabilities, observational limits, and conditions for resolving or failing to resolve claims about systems.            |

### Dependent and Integrative Theories

Dependent and integrative theories are built on other theories.
Deps lists direct SE theory dependencies, excluding transitive dependencies.

MM=MathlibMini, NS=neutral substrate, PS=persistence, TR=transformation,
IND=individuation, IR=identity regimes.

| Deps     | Repository                                                                                                                | Role in Structural Explainability                                                                                           |
| -------- | ------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| MM+NS    | [se-theory-common-ground](https://github.com/structural-explainability/se-theory-common-ground)                           | Conditions under which a bounded referential fragment is compatible with a class of interpretive frameworks.                |
| MM+NS+PS | [se-theory-individuation](https://github.com/structural-explainability/se-theory-individuation)                           | Conditions under which a presentation picks out one whole, and same-unit and distinct-unit judgments between presentations. |
| NS+PS    | [se-theory-coreference](https://github.com/structural-explainability/se-theory-coreference)                               | Context-indexed co-reference judgments, the identity they generate, and the distinct-commitments kept separate from them.   |
| PS+TR    | [se-theory-transformation-persistence](https://github.com/structural-explainability/se-theory-transformation-persistence) | Connections between transformation classifications and persistence semantics.                                               |
| NS+PS    | [se-theory-identity-regimes](https://github.com/structural-explainability/se-theory-identity-regimes)                     | Regime-relative identity criteria and their relationships to transformations.                                               |
| PS       | [se-theory-operational-identity](https://github.com/structural-explainability/se-theory-operational-identity)             | Relationships between declared identity semantics and identity behavior induced by implementations.                         |
| TBD      | [se-theory-interpretive-kernel](https://github.com/structural-explainability/se-theory-interpretive-kernel)               | Equivalence relationships and interpretation across distinct carriers.                                                      |
| NS+IR    | [se-theory-structural-explainability](https://github.com/structural-explainability/se-theory-structural-explainability)   | Integration of foundational SE concepts and their structural relationships.                                                 |

### Theory Infrastructure

| Repository                                                                                      | Role                                                                                                 |
| ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| [se-theory-reference-kit](https://github.com/structural-explainability/se-theory-reference-kit) | Shared validation, documentation, cataloging, and reference-artifact tooling for Lean theories.      |
| [se-protocols-research](https://github.com/structural-explainability/se-protocols-research)     | Scientific source audits, theory construction, independent review, and theory acceptance procedures. |

## Research Papers

Research papers develop and communicate the scientific and mathematical
foundations of Structural Explainability.

| Repository                                                                                                          | Subject                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------- |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate)             | SE-100: Neutral Substrates      |
| [paper-110-common-ground](https://github.com/structural-explainability/paper-110-common-ground)                     | SE-110: Common Ground           |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes)               | SE-200: Referential Regimes     |
| [paper-210-operational-identity](https://github.com/structural-explainability/paper-210-operational-identity)       | SE-210: Operational Identity    |
| [paper-220-interpretive-kernel](https://github.com/structural-explainability/paper-220-interpretive-kernel)         | SE-220: Interpretive Kernel     |
| [paper-320-structural-assurability](https://github.com/structural-explainability/paper-320-structural-assurability) | SE-320: Structural Assurability |

Formal claims and their verification should be evaluated against the
authoritative sources identified within each research repository.

## Research Pilots

Research pilots evaluate the applicability, explanatory value, and limitations
of SE concepts against concrete cases and external evidence.

| Repository                                                                                                                                                | Research Role                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| [se-pilot-individuation-comparison](https://github.com/structural-explainability/se-pilot-individuation-comparison)                                       | Source-grounded comparison of independently documented individuation accounts.                          |
| [se-pilot-identity-preservation-supply-chain-software](https://github.com/structural-explainability/se-pilot-identity-preservation-supply-chain-software) | Identity-preservation conformance across software supply-chain representations, including SBOM formats. |
| [se-pilot-structural-assurability](https://github.com/structural-explainability/se-pilot-structural-assurability)                                         | Applied investigation of assurance claims, evidence capabilities, and evaluation limitations.           |

<!--
| [se-regimes-pilot-education-math-g8](https://github.com/structural-explainability/se-regimes-pilot-education-math-g8) | Educational domain cases examining regime-relative identity and transformation behavior. |
-->

## Verification and Executable Research

These repositories provide executable constructions, independent checks,
or domain-specific verification.

| Repository                                                                                                                    | Role                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| [se-verification-self-similarity](https://github.com/structural-explainability/se-verification-self-similarity)               | Lean 4 mathematical cases testing individuation, co-reference, and persistence.      |
| [se-verification-operational-identity](https://github.com/structural-explainability/se-verification-operational-identity)     | Executable verification of finite Operational Identity constructions and algorithms. |
| [se-verification-vulnerability-matching](https://github.com/structural-explainability/se-verification-vulnerability-matching) | Examination of identity semantics in software vulnerability matching.                |
| [se-verification-judicial-record](https://github.com/structural-explainability/se-verification-judicial-record)               | Structural verification for accountable judicial record systems.                     |
| [se-interpretive-kernel](https://github.com/structural-explainability/se-interpretive-kernel)                                 | Executable finite interpretive-kernel constructions and witnesses.                   |

<!--
| [se-verification-civic-influence-record](https://github.com/structural-explainability/se-verification-civic-influence-record) | Structural verification for civic influence records. |
| [se-regimes](https://github.com/structural-explainability/se-regimes) | Executable identity-regime registry and transformation-response machinery. |
| [se-regimes-explorer](https://github.com/structural-explainability/se-regimes-explorer) | Interactive exploration of regime classifications and identity assumptions. |
-->

## SE Ecosystem Infrastructure

Shared specifications, contracts, registries, and tools support consistency
and traceability across repositories.

| Repository                                                                            | Role                                                                      |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| [se-manifest-schema](https://github.com/structural-explainability/se-manifest-schema) | Repository manifest schema and validation.                                |
| [se-constitution](https://github.com/structural-explainability/se-constitution)       | Common governance and structural rules for the SE ecosystem.              |
| [se-kernel](https://github.com/structural-explainability/se-kernel)                   | Shared structural primitives and invariant vocabulary.                    |
| [se-formal-contract](https://github.com/structural-explainability/se-formal-contract) | Machine-checked formal contracts for operational SE components.           |
| [se-mapspec](https://github.com/structural-explainability/se-mapspec)                 | Structural mapping vocabulary and correspondence rules.                   |
| [se-contract-kit](https://github.com/structural-explainability/se-contract-kit)       | Shared contract implementation and validation utilities.                  |
| [se-admin](https://github.com/structural-explainability/se-admin)                     | Repository administration and ecosystem consistency tooling.              |
| [se-codeowners](https://github.com/structural-explainability/se-codeowners)           | Projection of repository oversight metadata into GitHub CODEOWNERS files. |
| [spec-se](https://github.com/structural-explainability/spec-se)                       | Structural Explainability specification.                                  |
| [spec-se-appendix](https://github.com/structural-explainability/spec-se-appendix)     | Supporting disclosure and provenance appendix format.                     |

## Domain Applications and Mappings

These repositories apply SE structures and mapping concepts to external
domains and information systems.

| Repository                                                                                | Role                                                                        |
| ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| [se-df](https://github.com/structural-explainability/se-df)                               | Domain formalization toolkit.                                               |
| [se-mapping-assurance](https://github.com/structural-explainability/se-mapping-assurance) | Structural mappings between assurance frameworks and SE assurance concepts. |

<!--
| [se-mapping-education](https://github.com/structural-explainability/se-mapping-education) | Structural mappings for educational information. |
| [se-mapping-education-math](https://github.com/structural-explainability/se-mapping-education-math) | Mathematics education mapping models. |
| [se-mapping-education-math-g8](https://github.com/structural-explainability/se-mapping-education-math-g8) | Grade 8 mathematics mapping examples. |
| [scheduling-semantic-substrate](https://github.com/structural-explainability/scheduling-semantic-substrate) | Semantic substrate for scheduling records and changes. |
| [schedule-conformance](https://github.com/structural-explainability/schedule-conformance) | Conformance evaluation for scheduling representations. |
-->

Government-source repositories and other domain resources are available
through the [organization repository index](https://github.com/orgs/structural-explainability/repositories).

## How the Work Connects

Structural Explainability develops through related but distinct activities:

- **Papers** develop and communicate scientific arguments.
- **Theory repositories** formalize definitions, assumptions, and mathematical consequences.
- **Research pilots** investigate whether proposed concepts apply faithfully to independently documented cases.
- **Verification repositories** examine specified formal, algorithmic, or implementation properties.
- **Research protocols** govern source analysis, adversarial review, and scientific acceptance.

For example,
`se-theory-individuation` develops formal constructions concerning individuation,
while `se-pilot-individuation-comparison` investigates the
source-grounded comparison of individuation accounts.

<!-- markdownlint-enable MD024 -->
