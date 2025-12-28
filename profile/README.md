<p align="center">
  <img src="./logo_no_text.png" alt="Structural Explainability logo" width="220">
</p>

# Structural Explainability

This work develops foundational structural constraints on ontological substrates
intended to support accountability and interoperability 
under persistent interpretive disagreement.
It establishes what must be true of any such substrate 
prior to concrete ontology design or implementation.

### Foundational Results

| Artifact | Focus | Status | Description |
|--------|-------|--------|-------------|
| [NeutralSubstrate (Lean 4)](https://github.com/structural-explainability/NeutralSubstrate) | Ontological neutrality constraint | ![CI](https://github.com/structural-explainability/NeutralSubstrate/actions/workflows/ci.yml/badge.svg?branch=main) | Proves an impossibility result: substrates stable under incompatible extensions must be pre-causal and pre-normative. |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate) | Paper companion | Submitted | Narrative exposition of the neutrality theorem and its formal proof, establishing the design constraints for any neutral representational substrate. |
| [IdentityRegimes (Lean 4)](https://github.com/structural-explainability/IdentityRegimes) | Identity & persistence necessity | ![CI](https://github.com/structural-explainability/IdentityRegimes/actions/workflows/ci.yml/badge.svg?branch=main) | Shows that exactly six identity-and-persistence regimes are necessary and sufficient for accountability-oriented substrates under neutrality assumptions. |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes) | Paper companion | Submitted | Narrative exposition of the identity-regimes result and its formal justification. |


### Structural Constructions Enabled by the Foundational Results

| Artifact | Focus | Status | Description |
|--------|-------|--------|-------------|
| [AccountableEntities (Lean 4)](https://github.com/structural-explainability/AccountableEntities) | Entity-regime instantiation | ![CI](https://github.com/structural-explainability/AccountableEntities/actions/workflows/ci.yml/badge.svg?branch=main) | Formalizes the bijective mapping from named accountable entity kinds to the six identity-and-persistence regimes required by the framework. |
| ExchangeProtocol (Lean 4) | Neutral exchange substrate | ![CI](https://github.com/structural-explainability/ExchangeProtocol/actions/workflows/ci.yml/badge.svg?branch=main) | Defines neutral, time-parametric record structures (entities, relationships, exchanges, envelopes) for representing accountable exchanges without embedding causal, normative, or domain semantics. |
| Contextual Evidence & Explanations (CEE) | Explanation substrate | Draft | Specifies the neutral structural forms of explanations, evidence groupings, and contextual justification required for accountability under disagreement, without asserting causal models, normative judgments, or interpretive conclusions. |
| Interpretation & Conformance Boundary | Substrate-interpretation interface | Conceptual | Defines the boundary conditions under which external legal, ethical, or policy frameworks may interpret, constrain, or profile substrate records, without altering the neutral structural core or asserting normative conclusions. |

## Overview

Structural Explainability is a foundational research program
concerned with the design of **neutral representational substrates**
that preserve stable reference and accountability
under persistent disagreement.

The work develops structural constraints on ontology design
independently of domain, policy, or interpretive framework,
with a focus on identity, persistence, and extension stability.

## Scope

Structural Explainability addresses questions such as:

- What structural commitments are unavoidable if disagreement is persistent?
- How can accountability be represented without embedding causal or normative assumptions?
- What identity and persistence regimes are required for stable reference?

The results are theoretical and constraint-based.
They are not proposals for domain ontologies or protocols.

## Core Results

- Ontological neutrality requires pre-causal and pre-normative substrates
- Exactly six identity-and-persistence regimes are necessary and sufficient
  for neutral accountability under persistent disagreement

## Relationship to Civic Interconnect

Structural Explainability provides theoretical foundations that inform
the design of the Civic Interconnect ecosystem, including work on
Accountable Entities (AE), the Civic Exchange Protocol (CEP),
and Contextual Evidence and Explanations (CEE).
