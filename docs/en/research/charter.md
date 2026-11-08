# Structural Explainability Research Charter

## Charter Purpose

This charter keeps the research aimed at the key question.
It records what is frozen, what is tested, and what new work must show.
It is a decision document rather than an overview.
It is read at the start of each working session,
together with the organization profile/README.md and the boundaries index.

## Research Objective

Establish formal design constraints
under which shared information systems can preserve common referential records.
The same systems support multiple, possibly incompatible interpretations.
No one interpretation becomes foundational.
The constraints are independent of the technology used to implement a system.

Interpretation is welcome when it is stated, attributed, and open to dispute.

## Motivation Status

Some existing systems may not follow such constraints.
This has not been established as a finding.
No claim about how common this is is made without evidence.

## Test Question

Are the Neutral Substrate design constraints
mathematically justified, scientifically adequate, and
realizable in concrete information systems?
This includes systems built with existing ontology technologies.

## Obligations Under Test

Experiments test specific obligations:

- Referential fixing.
- Permitted attribution.
- Framework compatibility.
- Interpretive non-commitment.
- Extension stability.

Realizability can be investigated in two ways:

- Design a system directly against the constraints.
- Audit an existing system by representing its commitments
  with attribution and evaluating the applicable neutrality constraints.

Neither requires a general converter.
Showing one design complies does not show that all systems can be made neutral.

## Three Criteria

Every result states which criterion it bears on:

- **Mathematical correctness**: what is proved under the stated assumptions.
- **Scientific adequacy**: whether real designs can justify those assumptions and satisfy the constraints.
- **Theoretical contribution**: what the constraints establish beyond existing ontology architecture and knowledge representation.

Representing attributed claims in an existing technology is not itself a contribution.
Precise, independently justified conditions that
separate compliant from noncompliant designs could be.

## Frozen Foundations

For this phase, the theory repositories are treated as given.
Foundations are reopened only in response to documented evidence
of a defect, limitation, or inadequate assumption.
The issue is recorded in the owning repository's `DOUBTS.md`.
Discussion or implementation preference alone does not reopen a foundation.

See: each theory repository's `DOUBTS.md`.

## Admission Rule

### Experiments

Every experiment states the following before work begins:

- The obligation it tests, and the repository and definition that own it.
- The domain, the sources it uses, and
  whether those sources are constructed or independent.
- The result that would count against the obligation.

Experiments use existing mechanisms unless a demonstrated limitation prevents the test.

### Components

A new component, language, or tool must show why existing components are insufficient.
It is kept only if a demonstrated need requires it.
If any required item cannot be stated, the work may be parked.

## Evidence Rules

Evidence is kept in separate classes:

- Foundational sources.
- Construction cases.
- Adversarial cases.
- Independent application cases.

Adversarial cases and failure criteria are written
before any mapping or experiment is run.
Engineering validation is not held-out evidence.
Policies declared by the analyst are not independent systems that disagree.
Results apply only within the hypotheses stated where they are proved.

## Support and Failure

A mechanism gains empirical support
when the same core semantics operate unchanged
in two or more independently documented domains.
Support is subject to each domain's declared assumptions and limitations.
It is not a proof of general domain neutrality.

Failures to look for include:

- Unsupported attribution.
- Unjustified referential alignment.
- Commitments introduced silently.
- Source claims, or their source-relative consequences,
  that cannot be faithfully represented, retained, or
  recovered without introducing unsupported substrate commitments.
- Required neutrality conditions that cannot be established.

The substrate does not adopt the consequences of an imported interpretation.
Preserving the source claim and its context is the requirement.

A failure is diagnosed at its own layer.
Adapter and implementation failures are not automatically theoretical doubts.
A failure that bears on a foundation is recorded in the owning repository's `DOUBTS.md`.

## Reporting and Evaluation

Neutral mechanisms report attributed commitments, differences, and limitations.
They do not adopt an interpretation as shared truth.
Independent evaluations may assess conformance or correctness
under explicitly declared criteria.
Those assessments remain attributed and
do not become foundational commitments.

## Layering

Upstream theories do not mention downstream ones.
Pilots, verification, and tools depend on theories in one direction only.

See: the dependency tables in the organization README.

## Boundaries Index

The boundaries index lists exclusions, standing rules, and
doubts across the repositories.
Each entry carries its source repository, location, and link.
Existing identifiers and statuses are preserved where provided.
Resolved doubts include a one-line resolution.
Status comes from the source heading, such as open or resolved.
A resolved item also carries a one-line resolution.
The index is generated from the repositories, not written by hand.
No item is treated as open without checking its recorded status.

## Retiring Components

A component that fails the admission rule is archived, not deleted.
A component pinned by a frozen record stays resolvable at the pinned commit.

## Session Start

Read the organization README, this charter, and the boundaries index.
Check proposed work against the admission rule before building it.
