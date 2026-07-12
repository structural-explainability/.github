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

- **Identity & Persistence:** A stable, inspectable identity is the prerequisite
  for all tracking and provenance. Identity is _regime-relative_:
  a single structural change might preserve identity under one regime,
  break it under another, or be identity-neutral under a third.
- **Declared Identity Semantics:** A system that branches on an undeclared field to
  decide sameness is running a _hidden regime_.
  SE exists to detect hidden regimes.
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
| **Structural Explainability** | Integrates these layers into an explicit, explainable account without forcing consensus.                                                                             |
| **NS-Conformance**            | Decides, over a declared artifact, whether a deployed record system satisfies the substrate constraint.                                                              |

Within the core substrate, structure, transformation, persistence, and regime
behavior may be recorded.
Causal explanation, normative evaluation, authority,
legitimacy, obligation, and enforcement are not asserted as substrate-level commitments;
they may be attached through constrained downstream mechanisms.

### Protected Boundaries

Strict architectural boundaries protect this substrate
from leaking or collapsing into downstream application layers:

- _Governance Boundary (GB):_ Prevents operational records from implicitly
  transforming into claims of absolute authority, legitimacy, obligation, or enforcement.
- _Interpretation Boundary (IB):_ Ensures that external frameworks, explanations, and model interpretations
  remain attached as dynamic overlays rather than becoming hardcoded substrate semantics.
- _Attribution Boundary (REF / ATTR / EXT):_ Classifies exposed paths of a deployed
  record by the foundational commitment they carry: referential, attributive, or extension.
  This boundary is decidable and checked.

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
The system decides. It decides by branching on some field,
such as a version column, status flag,
or display attribute not necessarily declared as identity-relevant.

That is a _hidden regime_:
identity semantics implemented but not declared,
which may remain invisible until the system is challenged
in court, in audit, in appeal, in public review, or
in cross-institutional reconciliation.
By then, the records may already have committed to an identity model
not explicitly declared.

Existing infrastructure may not catch it.
Provenance models, content credentials, software bills of materials,
version control, and audit logs record what happened.
None answer what the system takes sameness to be, and none can detect a
system that answers it differently across undeclared fields.

Hidden regimes are findable, because the alternative is known in advance.
Six of the nine identity regimes sit in pairs on three sibling axes:
LOC/OBJ, SCOPE-E/SCOPE-S, RULE-C/RULE-S.
Each pair offers two admissible identity bases for the same kind of referent.

A hidden regime appears as a specific, finite thing:
a pair of records the declared regime treats as one referent,
the sibling regime treats as two,
and some field in the system already treats differently.
That pair is the witness and there is nothing to infer or interpret.

Accountable Records defines what a system must declare for this to be checked,
and gives the procedure.

SE does not replace domain vocabularies, standards, ontologies, or existing data systems.
It constrains how systems implement them so that disagreement remains
visible, attributable, and useful over time.

<details>
<summary>View the Neutral Record Methodology Approach</summary>

### The Neutral Record Approach

In information science, creating a **neutral record** means developing a
data schema, ontology, or knowledge graph that intentionally avoids
embedding specific subjective, cultural, or institutional norms into its core structure.

Traditional schemas often reflect the worldview of their creators.
This can make them rigid and bias data collection against different paradigms.

This research field aims to separate data syntax and structure from data semantics and interpretation.
The goal is to build highly flexible, semantic architectures,
via decentralized ledgers or modular metadata schemas,
where data can be ingested exactly as it exists or is reported.
The interpretations, values, and norms are then applied via dynamic overlays
or flexible querying layers, and are not hardcoded into the foundational ontology itself.

By separating the neutral substrate (what structurally happened)
from the interpretation boundary (claims made),
SE addresses a significant challenge in information ecosystems.

</details>

## Papers

The formal core of Structural Explainability is developed in three papers.
The papers are the normative specification.

| Paper      | Title                                                                                                 | arXiv                                          |
| ---------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| **SE-100** | Neutral Substrates: A Design Constraint for Shared Records Under Persistent Interpretive Disagreement | [2601.14271](https://arxiv.org/abs/2601.14271) |
| **SE-200** | Referential Regimes: Transformation-Invariant Identity for Neutral Substrates                         | [2601.16152](https://arxiv.org/abs/2601.16152) |
| **SE-300** | Accountable Records: NS-Conformance Checking for Transformation-Invariant Identity                    | _in preparation_                               |

**SE-100** establishes the neutrality-by-design constraint:
a substrate is neutral when its foundational layer is restricted
to referential commitments and permitted attribution propositions.

**SE-200** derives the referential-regime structure that neutral substrates require,
yielding six coarse families and nine core identity regimes:
OBL, OCC, REC, LOC, OBJ, SCOPE-E, SCOPE-S, RULE-C, RULE-S.

**SE-300** defines the _accountable record_,
the deployed artifact that declares its carrier, basis, regime,
transformation history, attribution boundary, and discriminator surfaces,
and provides checks that decide NS-conformance over it.

Conformance is three-valued:
PASS, FAIL, or INDETERMINATE.
An indeterminate result does not count as conformance.
Failures return finite witnesses, not scores.

Full conformance is disclosure-relative:
the checker decides over the declared artifact,
and a later undeclared-surface witness refutes the claim.

A parallel stewardship track addresses governance over time covering how neutral systems are
defined, audited, stressed, and repaired in real institutional contexts.

| Repository                                                                                                  | Focus               |
| ----------------------------------------------------------------------------------------------------------- | ------------------- |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate)     | Neutral substrates  |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes)       | Referential regimes |
| [paper-300-accountable-records](https://github.com/structural-explainability/paper-300-accountable-records) | Accountable records |

## NS-Conformance

NS-conformance is the checkable relation defined by SE-300. This is the layer at which
the theory meets a deployed system.

| Repository                                                                    | Purpose                                                                                                                                     |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| [ns-conformance](https://github.com/structural-explainability/ns-conformance) | Machine-readable schemas for the accountable-record bundle, the reference checker for the NS-conformance checks, and the conformance suite. |

An **accountable-record bundle** supplies the following artifacts:

1. a carrier-basis-regime profile;
2. record identifiers and payload references;
3. typed transformation histories;
4. attribution-boundary declarations;
5. a discriminator-surface registry; and
6. a disclosure attestation identifying the implementation boundary.

The **checker** consumes a bundle and returns a conformance report:
per-record and per-store results, the effective declarations used by each check,
normalized histories, and every failure and indeterminate witness.

The **conformance suite** is a set of bundles with known verdicts
sufficient to validate an independent implementation of the checks.
It allows checkers to be tested and falsified.

Bundles may be produced directly, or emitted by adapters over existing provenance graphs,
version-control systems, schema registries, workflow engines, and audit logs.
Adapters are not part of the specification.

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
  RR --> AR[Accountable Records]
  AR --> NC[ns-conformance]
```

## How to Use This Organization

- **To understand the theory**, read the three papers.
- **To check a declared record system**, use `ns-conformance`.

<!-- markdownlint-enable MD024 -->
