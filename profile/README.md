# Structural Explainability

<!-- markdownlint-disable MD024 -->

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/.github/actions/workflows/ci-hygiene.yml/badge.svg?branch=main)
[![Check Links](https://github.com/structural-explainability/.github/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/.github/actions/workflows/links.yml)

> Defines the neutral constraints under which systems remain explainable,
> inspectable, and contestable without embedding interpretation.

## Core Statement

Structural Explainability (SE) defines a neutral structural substrate for recording
identity, structure, transformation, and change without embedding interpretation,
authority, causality, or judgment.

Structural Explainability is not anti-interpretation; it is anti-implicit interpretation.
It separates structural facts from downstream claims so interpretation and
disagreement can remain explicit, attributable, and contestable over time.

Record systems commit to identity semantics.
When a rule is refined, an agent redeployed, a jurisdiction subdivided,
or two records merged, the system decides whether the thing is still the same thing.
That decision is load-bearing for citation, liability, and audit, but not always declared.

SE makes the commitment declarable and the failure detectable.

### The Foundational Core

- **Identity & Persistence:** Persistent tracking and provenance depend on
  inspectable identity conditions. Identity is _regime-relative_:
  a single structural change might preserve identity under one regime,
  break it under another, or be identity-neutral under a third.
- **Declared Identity Semantics:** A system may induce a rule of sameness
  through an audited implementation surface based on one registered artifact
  or on a joint mechanism over several registered artifacts.
  SE makes divergence from the declared rule detectable as a finite witness
  and separates detection from sibling diagnosis and regime substitution.
- **Plural Systems:** SE is built for independent architectures
  that share data without requiring a centralized authority,
  uniform naming, or a single forced ontology.

### The Architecture Stack

| Layer                         | Function                                                                                                                                                             |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Neutral Substrate**         | Defines admissible structural description without interpretive commitment.                                                                                           |
| **Transformation Theory**     | Identifies and defines structural change pressures.                                                                                                                  |
| **Persistence Theory**        | Classifies each transformation, relative to an identity regime, as identity-preserving (PRS), identity-breaking (BRK), identity-neutral (NEU), or inapplicable (NA). |
| **Identity Regimes**          | Organizes identity and persistence behavior into nine core identity regimes.                                                                                         |
| **Operational Identity**      | Compares the declared identity partition with operational partitions induced by audited surfaces, exposing divergence as a finite witness.                           |
| **Structural Explainability** | Integrates these layers into an explicit, explainable account without forcing consensus.                                                                             |

Within the core substrate, structure, transformation, persistence, and regime
behavior may be recorded.
Causal explanation, normative evaluation, authority,
legitimacy, obligation, and enforcement are not asserted as substrate-level commitments;
they may be attached through constrained downstream mechanisms.

Downstream domains (e.g., law, infrastructure, agentic AI systems)
consume the core substrate without redefining it.
SE records the structural commitments of a system without deciding their ultimate meaning,
enabling continuous cross-institutional coordination through persistent disagreement.

## Overview

Some information systems make decisions that affect people, attribute claims to
sources, record contested facts, or coordinate across institutions that disagree.
Those systems can hold a compliance conclusion, a legal holding, or a causal claim
while every party continues to refer to the same underlying artifacts.

They fail in a specific way.
Under change, the system must decide what stays the same:
whether a refined rule is the same rule,
whether a redeployed agent is the same agent,
whether a subdivided scope is the same scope.
The implementation answers through fields, predicates, workflow states,
configuration values, or joint mechanisms over several registered artifacts.
Identity-relevant uses of those mechanisms may induce
an operational identity partition that differs from the declared identity partition.

That divergence may remain invisible until the system is challenged
in court, in audit, in appeal, in public review, or in cross-institutional reconciliation.
By then, the records may already have committed to an identity model not explicitly declared.

Existing infrastructure may not catch it.
Provenance models, content credentials, software bills of materials,
version control, and audit logs record what happened.
They do not necessarily require a system to declare its rule of sameness
or compare that declaration against the
identity relation induced by its implementation.

Six of the nine identity regimes sit in pairs on three sibling axes:
LOC/OBJ, SCOPE-E/SCOPE-S, RULE-C/RULE-S.
Each pair offers two admissible identity bases for the same kind of referent.
When a sibling basis is available and also splits an examined declared class,
the divergence can be classified against it;
otherwise, the divergence is unpositioned.

A divergence has a specific, finite witness:
a pair of records the declared partition places together and an audited surface separates.
That pair is the witness.
The witness alone does not establish the divergence's sibling classification
or which identity basis the surface carries.
A surface implements a hidden identity regime only when
the sibling differs from the declared regime on the examined domain
and the operational partition equals the sibling partition there.

Operational Identity defines what a system must declare for this to be checked,
and gives the procedure.

SE does not replace domain vocabularies, standards, ontologies, or existing data systems.
It constrains how systems implement them so that disagreement remains
visible, attributable, and useful over time.

## Papers

The formal core of Structural Explainability is developed in three papers.
The papers are the normative specification.

| Paper      | Title                                                                                                 | arXiv                                          |
| ---------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| **SE-100** | Neutral Substrates: A Design Constraint for Shared Records Under Persistent Interpretive Disagreement | [2601.14271](https://arxiv.org/abs/2601.14271) |
| **SE-200** | Referential Regimes: Transformation-Invariant Identity for Neutral Substrates                         | [2601.16152](https://arxiv.org/abs/2601.16152) |
| **SE-210** | Operational Identity: A Finite Audit of Declared and Implemented Rules of Sameness                    | _draft_                                        |

**SE-100** establishes the neutrality-by-design constraint:
a substrate is neutral when its foundational layer is restricted
to referential commitments and permitted attribution propositions.

**SE-200** derives the referential-regime structure that neutral substrates require,
yielding six reference kinds and nine core identity regimes:
OBL, OCC, REC, LOC, OBJ, SCOPE-E, SCOPE-S, RULE-C, RULE-S.

**SE-210** defines the operational identity partition,
the rule of sameness induced by an examined implementation surface,
and gives a finite audit comparing it against the declared partition.
The paper specifies the finite audit inputs:
the examined record domain and declared regime,
the family-labeled transformation history,
the identified implementation boundary and registered artifacts,
the evaluated surfaces over those artifacts,
the identity-relevant uses identified for each surface,
and the corresponding completeness claims.

| Repository                                                                                                    | Focus                |
| ------------------------------------------------------------------------------------------------------------- | -------------------- |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate)       | Neutral substrates   |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes)         | Referential regimes  |
| [paper-210-operational-identity](https://github.com/structural-explainability/paper-210-operational-identity) | Operational Identity |

## Repository Manifests

SE repositories use manifests to describe the repository's role, scope, dependencies,
provided artifacts, validation expectations, governance, and traceability.

The SE manifest complements external metadata standards.
Citation metadata belongs in `CITATION.cff`;
software supply-chain metadata may use SPDX;
software discovery metadata may use CodeMeta;
research-object packaging may use RO-Crate.

| Repository                                                                            | Purpose                                        |
| ------------------------------------------------------------------------------------- | ---------------------------------------------- |
| [se-manifest-schema](https://github.com/structural-explainability/se-manifest-schema) | Canonical manifest schema for SE repositories. |

## Dependency Chain

```mermaid
flowchart LR
  NS[Neutral Substrates] --> RR[Referential Regimes]
  RR --> OI[Operational Identity]
```

## How to Use This Organization

- **To understand the theory**, read the three papers.
- **To check a declared record system**, apply the Operational Identity audit from SE-210.

<!-- markdownlint-enable MD024 -->
