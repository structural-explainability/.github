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

### The Foundational Core

- **Identity & Persistence:** A stable, inspectable identity is the prerequisite
  for all tracking and provenance. Identity is _profile-relative_:
  a single structural change might preserve identity under one profile,
  break it under another, or be entirely irrelevant under a third.
- **Plural Systems:** SE is built for independent architectures
  that share data without requiring a centralized authority,
  uniform naming, or a single forced ontology.

### The Architecture Stack

| Layer                         | Function                                                                                           |
| :---------------------------- | :------------------------------------------------------------------------------------------------- |
| **Neutral Substrate**         | Defines admissible structural description without interpretive commitment.                         |
| **Transformation Theory**     | Identifies and defines structural change pressures.                                                |
| **Persistence Theory**        | Determines profile-relative preservation (PRS), breakage (BRK), or irrelevance (IGN) under change. |
| **Identity Regimes**          | Organizes identity and persistence behavior into nine referential profile kinds.                   |
| **Structural Explainability** | Integrates these layers into an explicit, explainable account without forcing consensus.           |

Within the core substrate, structure, transformation, persistence, and profile
behavior may be recorded.
Causal explanation, normative evaluation, authority,
legitimacy, obligation, and enforcement are not asserted as substrate-level commitments;
they may be attached through constrained downstream mechanisms.

### Protected Boundaries

Two strict architectural boundaries protect this substrate
from leaking or collapsing into downstream application layers:

- _Governance Boundary (GB):_ Prevents operational records from implicitly
  transforming into claims of absolute authority, legitimacy, obligation, or enforcement.
- _Interpretation Boundary (IB):_ Ensures that external frameworks, explanations, and model interpretations
  remain attached as dynamic overlays rather than becoming hardcoded substrate semantics.

Downstream domains (e.g., law, infrastructure, agentic AI systems)
consume the core substrate without redefining it.
SE records the structural commitments of a system without deciding their ultimate meaning,
enabling continuous cross-institutional coordination through persistent disagreement.

## Overview

Some information systems make decisions that affect people, attribute claims to
sources, record contested facts, or coordinate across institutions that disagree.
When those systems collapse what should be distinct layers (what is structurally recorded,
what is governed, what is interpreted, what is attested) into a single record,
they lose the ability to represent the disagreement they exist to handle.

That collapse is often invisible until the system is challenged:
in court, in audit, in appeal, in public review, or
in cross-institutional reconciliation.
By then, the records may already have committed to interpretations,
authority claims, or judgments that the system never explicitly declared.

Structural Explainability defines the structural conditions under which this
collapse can be prevented.
It identifies what must be kept separate for an information system
to remain durable, inspectable, and contestable under persistent disagreement:

- identity from graph continuity
- attribution from authority
- governance status from correctness
- evidence from interpretation
- dependency from validity
- explanation from proof
- record from judgment

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
This makes them rigid and biases the data collection against different paradigms.

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

## Operational Security: Capability vs. Authority

Before looking at the tooling implementations,
it is critical to see how SE's non-collapse discipline applies to the development environment itself.
Just as the data substrate must not collapse history into interpretation,
the operational environment must not collapse technical permissions into semantic authority.

## Capability Is Not Authority

> A protected surface is one where the technical capability to change it
> is not the authority to change it.

Access control can grant the capability to perform an operation.
It does not by itself establish that the capability is sufficient authority
to modify a protected repository or lifecycle surface.

Accountable Surfaces records where capability is insufficient authority,
and binds each crossing of that gap to required human review, supporting evidence,
and permitted AI participation.

The authority manifest is self-protecting because the alternative is the
collapse it exists to prevent: if an actor with technical capability can rewrite
the authority declaration, capability has silently become authority.

## Repository Authority Surfaces

SE repositories may additionally declare an authority manifest at
`.accountability/surfaces.toml`, a sibling to `SE_MANIFEST.toml`.

Where `SE_MANIFEST.toml` declares structural role, scope, and dependencies,
the authority manifest declares which repository and lifecycle surfaces are
authority-bearing: surfaces a tool may be technically able to change but is
not legitimately authorized to change without review.

This layer is operational, not substrate.
It records declared review and evidence requirements for repository surfaces.
It does not confer authority, legitimacy, obligation, or enforcement as substrate facts,
and it respects the Governance Boundary.
Enforcement is external and lives with `se-admin` tooling.

It applies SE's non-collapse discipline to the authority layer:
technical capability is separated from legitimate authority,
as record is separated from judgment.
AI systems may assist review but may not satisfy human review authority.

The authority manifest is itself a protected surface.
It requires human review and evidence of review,
and AI authority over it is prohibited.

| Repository                                                                                                        | Purpose                                                                                                |
| ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [accountable-surface-spec](https://github.com/structural-explainability/accountable-surface-spec)                 | Source of truth for `.accountability/surfaces.toml` structure                                          |
| [accountable-authority-vocabulary](https://github.com/structural-explainability/accountable-authority-vocabulary) | Permission, AI authority level, and revocation terms                                                   |
| [accountable-surface-vocabulary](https://github.com/structural-explainability/accountable-surface-vocabulary)     | Surface object, role, lifecycle gate, downstream effect                                                |
| [accountable-evidence-vocabulary](https://github.com/structural-explainability/accountable-evidence-vocabulary)   | Evidence and verification terms                                                                        |
| [accountable-review-vocabulary](https://github.com/structural-explainability/accountable-review-vocabulary)       | Review, review scope, and reviewer authority terms                                                     |
| [se-codeowners](https://github.com/structural-explainability/se-codeowners)                                       | CLI utility that projects accountable surface declarations into GitHub CODEOWNERS and checks for drift |

The project `se-codeowners` is an enforcement projection,
not the source of authority.
The authority declaration remains `.accountability/surfaces.toml`;
`se-codeowners` renders one GitHub-specific expression of that declaration
by mapping oversight roles to CODEOWNERS entries.
This supports ordinary repository governance without collapsing
technical write capability into legitimate review authority.

## Accountable Agents

Accountable Agents extends the same non-collapse discipline to agentic AI systems.

An agent system may have technical capability:
it may observe, interpret, propose, modify, execute, transmit,
or self-alter depending on its product wrapper, execution environment,
tools, and permissions.
Some systems may also be configured near approval surfaces,
such as merge, release, deployment, certification, or risk acceptance.

That capability is not authority.
Responsibility cannot rest with an agent system; agent systems are tools.
Authority and accountability remain with the people and institutions
that use, build, release, deploy, authorize, operate, and review the systems.

This work is data-focused.
It works alongside existing standards, security guidance,
provenance models, model cards, product documentation, and research.
It links them through claim-level records so that agent capabilities,
affected surfaces, evidence sources, risk mappings, and
accountability requirements can be inspected together.

| Repository                                                                                          | Purpose                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [accountable-agents](https://github.com/structural-explainability/accountable-agents)               | Conceptual model for accountable agent systems, capabilities, execution environments, authority grants, evidence, review gates, protected surfaces, and accountable entities.       |
| [agent-capability-registry](https://github.com/structural-explainability/agent-capability-registry) | Reusable vocabulary for capability kinds, observable resources, effectable resources, capability levels, evidence statuses, mapping kinds, risks, mitigations, and standards links. |
| [agent-capability-mappings](https://github.com/structural-explainability/agent-capability-mappings) | Source-linked claims mapping specific products, models, versions, modes, execution environments, tools, and permissions to documented or inferred capabilities.                     |

## Shared Contract Tooling

Shared contract tooling supports packaging, validation, and distribution of
machine-readable contract artifacts across SE repositories.

| Repository                                                                      | Purpose                                                                                  |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| [se-contract-kit](https://github.com/structural-explainability/se-contract-kit) | Shared Python tooling for packaging, validating, and distributing SE contract artifacts. |

## Accountable Record Contract

| Repository                                                                            | Purpose                                                                                                                                     |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| [accountable-record](https://github.com/structural-explainability/accountable-record) | Language-neutral, data-first Accountable Record contract for bundles, profiles, reports, conformance, packages, and verification semantics. |

## Accountable Record Systems

Accountable Record systems apply SE constraints to durable record
structures.

The Accountable Record system repositories are in **active development**.
They track main on their SE dependencies during this phase to allow the
contract, domain systems, and verification implementations to co-evolve.
Pinned versions follow once the contract stabilizes.

Accountable Record systems produce durable, inspectable records of decisions,
relationships, claims, dependencies, sources, interpretations, or processes in
ways that support inspection, contestation, audit, and continued use under
disagreement.

These are application-layer repositories.
They are real systems, not demonstrations, built to use ordinary domain
vocabularies while preserving the structural distinctions required for
accountable verification.
These systems are organized as domain record systems,
jurisdiction-specific specializations, and
verification implementations.

### Domain Record Systems

Domain record systems implement the Accountable Record contract using ordinary
domain vocabularies.

These repositories define general domain profiles, packages, mappings, record
types, fixtures, and expected reports.
They are not limited to one jurisdiction, institution, dataset, or source system.

| Repository                                                                                  | Purpose                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [infrastructure-record](https://github.com/structural-explainability/infrastructure-record) | General infrastructure record system for assets, facilities, networks, inspections, dependencies, maintenance, incidents, operational state, source observations, and infrastructure record reports. |
| [energy-record](https://github.com/structural-explainability/energy-record)                 | General energy record system for generation, storage, hydrogen, transmission, distribution, interconnection, outage, reliability, emissions, dependencies, model outputs, and energy record reports. |
| [judicial-record](https://github.com/structural-explainability/judicial-record)             | General judicial record system for decisions, opinions, claims, holdings, citations, dependencies, later treatment, procedural history, source spans, and judicial record reports.                   |
| [civic-record](https://github.com/structural-explainability/civic-record)                   | General civic record system for people, organizations, roles, meetings, documents, relationships, funding, actions, sources, decisions, and civic records.                                           |

<details>
<summary>View Sector Mappings & Custom Extensions (Infrastructure, Civic, Education)</summary>

#### Extended Asset Implementations

- **General Infrastructure Records:** Shared definitions covering physical locations,
  routing linkages, systemic states, and operations.
- **Sector-Specific Specializations:** Extends downstream objects to `water-record`,
  `telecommunications-record`, `transportation-record`, and `waste-record` layouts.
- **Digital-Twin Linking:** Maps physical operational telemetry streams
  directly to logical models and underlying assumptions.

#### Jurisdiction Specialization Modules

- [judicial-record-us-federal-supreme](https://github.com/structural-explainability/judicial-record-us-federal-supreme) -
  Dedicated target data logic patterns optimized for US Supreme Court
  dockets, briefs, citations, and structured procedural records.

#### Local Public Domain Architectures

- `municipal-record` - budget definitions, ordinances, and council tracking paths.
- `municipal-contract-record` - public procurement validation loops from bids to performance.
- `public-meeting-record` - verifiable trace layouts for voting outcomes and agendas.
- `public-budget-record` - tracing fund appropriations without collapsing authority structures.

#### Academic Schema Extensions

- `education-record` - handles multi-jurisdictional criteria frameworks,
  competency matrices, tracking standards alignment histories, and
  systemic adoptions without merging disparate semantic interpretations.

</details>

## Accountable Record Verification Implementations

Verification tools consume contracts, layouts, and conformance metrics
to guarantee boundaries remain cleanly separated under load.

Structural Explainability does not replace domain ontologies or standards.
Domain systems may use
[Akoma Ntoso](https://www.oasis-open.org/standard/akn-v1-0/),
[LegalRuleML](https://docs.oasis-open.org/legalruleml/legalruleml-core-spec/v1.0/legalruleml-core-spec-v1.0.html),
[other OASIS open standards](https://www.oasis-open.org/standards/),
[FAIR principles](https://www.nature.com/articles/sdata201618),
[CIDOC-CRM](https://cidoc-crm.org/),
[schema.org](https://schema.org/) vocabularies, or other domain standards.

Verification checks whether a system's use of its chosen standards preserves
the distinctions needed for accountable representation under persistent
disagreement. It does not decide truth, legal correctness, civic authority,
institutional legitimacy, or final domain meaning.

| Repository                                                                                  | Purpose                                                                                                                                  |
| ------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | --- |
| [accountable-record-py](https://github.com/structural-explainability/accountable-record-py) | Core Python test engine driving contract assertions, lock packaging, profiles tracking, and automated verification validation reporting. |
| [judicial-record-py](https://github.com/structural-explainability/judicial-record-py)       | Custom Python verifier tooling checking judicial-record conformance metrics, text fixtures, and tracking validation sheets.              |
| [civic-record-py](https://github.com/structural-explainability/civic-record-py)             | Target verification architecture generating compliance matrix checks for active public institution profiles.                             |     |

## Mathematical Foundations & Proof Chains

<details>
<summary>View Category Theory Math, Lean 4 Theorems, and Specifications</summary>

### Theory (Formal Derivation Layer)

These repositories contain evolving Lean 4 theorem development
that derives and justifies the formal contract.
They are not consumed directly by operational systems.

| Repository                                                                                                              | Purpose                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| [se-theory-reference-kit](https://github.com/structural-explainability/se-theory-reference-kit)                         | Shared Python tooling for scaffolding, validating, inspecting, and exporting theory-reference artifacts that mirror Lean public surfaces            |
| [se-theory-neutral-substrate](https://github.com/structural-explainability/se-theory-neutral-substrate)                 | Formal development of the neutral-substrate constraint and admissible structure                                                                     |
| [se-theory-transformation](https://github.com/structural-explainability/se-theory-transformation)                       | Defines change pressure and foundational transformation operators, families, composition relations, orthogonality relations, and outcome vocabulary |
| [se-theory-persistence](https://github.com/structural-explainability/se-theory-persistence)                             | Defines preservation, breakage, and irrelevance under admissible transformation                                                                     |
| [se-theory-identity-regimes](https://github.com/structural-explainability/se-theory-identity-regimes)                   | Defines regime-specific identity and persistence behavior using nine refined referential profile kinds                                              |
| [se-theory-structural-explainability](https://github.com/structural-explainability/se-theory-structural-explainability) | Explains the resulting judgment without collapsing disagreements                                                                                    |

### Formal Contract and Operational Foundations

| Repository                                                                            | Purpose                                                                                              |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| [se-formal-contract](https://github.com/structural-explainability/se-formal-contract) | Lean 4-verified formal contract exporting invariants, regimes, and constraints to operational layers |
| [se-constitution](https://github.com/structural-explainability/se-constitution)       | Canonical schema, rules, and validation framework (consumes formal contract)                         |
| [se-admin](https://github.com/structural-explainability/se-admin)                     | Shared automation, scaffolding, and enforcement                                                      |
| [se-kernel](https://github.com/structural-explainability/se-kernel)                   | Core structural primitives and invariants (constrained by constitution and formal contract)          |
| [se-mapspec](https://github.com/structural-explainability/se-mapspec)                 | Mapping vocabulary and cross-system semantics (constrained by formal contract relations)             |

### Regime Execution

| Repository                                                                                                            | Purpose                                                              |
| --------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| [se-regimes](https://github.com/structural-explainability/se-regimes)                                                 | Executable regime kernel (profiles, transformations, verdicts)       |
| [se-regimes-pilot-education-math-g8](https://github.com/structural-explainability/se-regimes-pilot-education-math-g8) | Grade 8 mathematics regime pilot for linear equations and statistics |
| [se-regimes-explorer](https://github.com/structural-explainability/se-regimes-explorer)                               | SE Regimes Decision Tree                                             |

### Mapping Examples

| Repository                                                                                                | Purpose                                                                         |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| [se-mapping-education](https://github.com/structural-explainability/se-mapping-education)                 | Education standards mapping examples across jurisdictions and reference systems |
| [se-mapping-education-math](https://github.com/structural-explainability/se-mapping-education-math)       | Mathematics standards mapping examples using central atomic competency units    |
| [se-mapping-education-math-g8](https://github.com/structural-explainability/se-mapping-education-math-g8) | Grade 8 mathematics pilot mappings for linear equations and statistics          |

### Source Materials (govsrc)

| Repository                                                                                                      | Purpose                                      |
| --------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| [se-govsrc-us](https://github.com/structural-explainability/se-govsrc-us)                                       | All U.S. source materials                    |
| [se-govsrc-us-missouri](https://github.com/structural-explainability/se-govsrc-us-missouri)                     | Missouri-specific source materials           |
| [se-govsrc-us-education](https://github.com/structural-explainability/se-govsrc-us-education)                   | U.S. education source materials              |
| [se-govsrc-us-missouri-education](https://github.com/structural-explainability/se-govsrc-us-missouri-education) | Missouri education source materials          |
| [se-govsrc-finland-education](https://github.com/structural-explainability/se-govsrc-finland-education)         | Finland national curriculum source materials |
| [se-govsrc-norway-education](https://github.com/structural-explainability/se-govsrc-norway-education)           | Norway curriculum (LK20) source materials    |
| [se-govsrc-singapore-education](https://github.com/structural-explainability/se-govsrc-singapore-education)     | Singapore syllabus source materials          |
| [se-govsrc-oecd-pisa](https://github.com/structural-explainability/se-govsrc-oecd-pisa)                         | OECD PISA framework and assessment materials |

### Normative and Informative Specifications

| Repository                                                                        | Purpose                                                                 | Status      |
| --------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------- |
| [spec-se](https://github.com/structural-explainability/spec-se)                   | Neutrality and boundary constraints for all downstream systems          | Normative   |
| [spec-ae](https://github.com/structural-explainability/spec-ae)                   | Accountable entity kinds; references canonical identity-regime profiles | Normative   |
| [spec-ep](https://github.com/structural-explainability/spec-ep)                   | Graph evolution over accountable entities                               | Normative   |
| [spec-cee](https://github.com/structural-explainability/spec-cee)                 | Contextual evidence, explanation, attestation, and provenance           | Normative   |
| [spec-gb](https://github.com/structural-explainability/spec-gb)                   | Governance boundary for structural artifacts and actions                | Normative   |
| [spec-ib](https://github.com/structural-explainability/spec-ib)                   | Interpretation boundary for external frameworks                         | Normative   |
| [spec-se-appendix](https://github.com/structural-explainability/spec-se-appendix) | Identifier rules, examples, and cross-spec patterns                     | Informative |

### Optional Reference Implementations and Formal Anchors

| Repository                                                                                    | Purpose                       | Description                                                                                       |
| --------------------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------------- |
| [AccountableEntities](https://github.com/structural-explainability/AccountableEntities)       | Accountable entity kinds      | Lean formalization of six AE entity kinds and their mapping to canonical identity-regime profiles |
| [EvolutionProtocol](https://github.com/structural-explainability/EvolutionProtocol)           | Graph evolution over entities | Formalization of EP graph evolution                                                               |
| [CEE](https://github.com/structural-explainability/CEE)                                       | Evidence interface            | Structural forms for contextual explanation, evidence, attestation, and provenance                |
| [GovernanceBoundary](https://github.com/structural-explainability/GovernanceBoundary)         | Governance boundary           | Structural boundary for governance artifacts and actions                                          |
| [InterpretationBoundary](https://github.com/structural-explainability/InterpretationBoundary) | Interpretation boundary       | Conditions under which external frameworks may interpret substrate records                        |

### Archived / Superseded Theory Repositories

| Repository                                                                                        | Purpose                      | Description                                                                                                                     |
| ------------------------------------------------------------------------------------------------- | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| [StructuralExplainability](https://github.com/structural-explainability/StructuralExplainability) | Cross-cutting constraints    | Neutrality and conformance predicates                                                                                           |
| [NeutralSubstrate](https://github.com/structural-explainability/NeutralSubstrate)                 | Neutral-substrate constraint | Earlier formalization of the constraint that substrate-level commitments exclude object-level causal and normative propositions |
| [IdentityRegimes](https://github.com/structural-explainability/IdentityRegimes)                   | Referential regimes          | Earlier formalization of identity-and-persistence regime families prior to the current nine-profile refinement                  |

</details>

## Contract Derivation and Enforcement Chain

```mermaid
flowchart TD

  %% --- Theory Layer ---
  subgraph T[Theory Layer]
    NS[neutral substrate]
    TR[transformation]
    PE[persistence]
    IR[identity regimes]
    SET[structural explainability]
  end

  %% --- Boundary Specs ---
  subgraph B[Boundary Specs]
    GB[governance boundary]
    IB[interpretation boundary]
  end

  %% --- Contract / Governance ---
  subgraph G[Contract and Governance]
    FC[se-formal-contract]
    C[se-constitution]
    A[se-admin]
  end

  %% --- Operational Core ---
  subgraph O[Operational Core]
    K[se-kernel]
    M[se-mapspec]
    R[se-regimes]
    MAP[se-mapping-*]
    GOV[se-govsrc-*]
  end

  %% --- Accountable Record Systems ---
  subgraph ARS[Accountable Record Systems]
    AR[accountable-record]
    JR[judicial-record]
    CR[civic-record]
    JRS[Supreme Court specialization]
  end

  %% --- Verification Implementations ---
  subgraph V[Verification Implementations]
    ARPY[accountable-record-py]
    JRPY[judicial-record-py]
    CRPY[civic-record-py]
  end

  NS --> FC
  TR --> FC
  PE --> FC
  IR --> FC
  SET --> FC

  GB --> C
  IB --> C

  FC --> C
  C --> A

  A --> K
  A --> M
  A --> R
  A --> MAP
  A --> GOV

  K --> AR
  M --> AR
  R --> AR

  AR --> JR
  AR --> CR
  JR --> JRS

  ARPY --> AR
  JRPY --> JR
  CRPY --> CR

  IB -.-> AR
  IB -.-> JR
  IB -.-> CR

  GB -.-> AR
  GB -.-> JR
  GB -.-> CR
```

All repositories in this diagram declare an `SE_MANIFEST.toml` conforming to
[`se-manifest-schema`](https://github.com/structural-explainability/se-manifest-schema),
which has no upstream SE dependencies.

## Papers

Structural Explainability consists of a small formal core (SE-100: Neutral Substrates; SE-200: Referential Regimes)
and a parallel stewardship track addressing governance over time.
The stewardship track examines how neutral systems are defined, audited, stressed, and
repaired in real institutional contexts.

The two formal papers provide theoretical justification for foundational specifications.
They are explanatory rather than normative (they describe what must be true for such systems to work,
not what people should believe or do).

| Repository                                                                                              | Focus               | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------- |
| [paper-100-neutral-substrate](https://github.com/structural-explainability/paper-100-neutral-substrate) | Neutral substrates  | Neutral-substrate design constraint for shared records under persistent interpretive disagreement                   |
| [paper-200-identity-regimes](https://github.com/structural-explainability/paper-200-identity-regimes)   | Referential regimes | Referential-regime structure required by neutral substrates, deriving six coarse families and nine refined profiles |

## How to Use This Organization

- **To understand the justification**, start with the papers.
- **To understand the architecture**, start with the specifications.
- **To verify formal coherence**, consult the Lean formalizations.
- **To consume stable definitions**, use the formal contract artifacts.
- **To validate repositories**, use the manifest and conformance tooling.

<!-- markdownlint-enable MD024 -->
