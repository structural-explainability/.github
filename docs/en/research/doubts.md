# Research Doubts and Open Questions

This document records known
limitations, unresolved questions, and potential weaknesses
in the repository theory.

A doubt is not necessarily an error.
It's a question worth keeping visible so
we don't claim more than the evidence supports.

Some doubts can be resolved through mathematical proof.
Others require scientific examples, comparisons with existing work, or
better explanations of what the results mean.

The objective is to distinguish what we have established
from what remains to be demonstrated.

## Repository Summary

| Criterion                | Current assessment |
| ------------------------ | ------------------ |
| Mathematical Correctness | ...                |
| Scientific Adequacy      | ...                |
| Theoretical Contribution | ...                |

The doubts below identify specific issues affecting these assessments.

---

<!-- markdownlint-disable MD024 -->

## Register 1. Doubts About Assumptions (Undermining Doubts)

These questions concern the premises of an argument.

Even if a theorem is correctly proved, can we establish the assumptions necessary to apply it?

## Register 2. Doubts About Conclusions (Rebutting Doubts)

These questions concern whether a claimed conclusion is false.

For example, a counterexample satisfying all the premises
but violating the conclusion would challenge the claimed theorem or its formalization.

**None currently identified.**

A model that violates a required assumption does not
necessarily refute a conditional theorem.

If a counterexample is found,
we must identify the exact claim it challenges and
whether its assumptions are satisfied.

## Register 3. Doubts About What Our Results Mean (Undercutting Doubts)

These questions concern the connection
between a formal theorem and the scientific claim made about it.

A theorem may be correct while its informal interpretation is too strong.

Some of these doubts are addressed by permanent documentation
rules rather than additional proofs.

<!-- markdownlint-enable MD024 -->

## Guide

State what is proved,
what is supported by evidence, and
what remains uncertain.
A known limitation is not a failure when accurately identified and respected.

## Research Criteria

We evaluate Structural Explainability research against three criteria.

| Criterion                       | Asks                                                                                                     |
| ------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **1. Mathematical Correctness** | Are definitions precise, assumptions explicit, and claimed mathematical results correctly proved?        |
| **2. Scientific Adequacy**      | Do definitions, assumptions, and models meaningfully represent the phenomena we intend to study?         |
| **3. Theoretical Contribution** | Does the work establish something new and significant, beyond restating assumptions or existing results? |

These criteria are related, and satisfying one does not establish the others.

### Criteria 1. Mathematical Correctness

Lean checks whether a formal theorem follows from
its stated assumptions and the underlying logical rules.
It can also establish that assumptions are jointly satisfiable
by verifying a model in which they all hold.

However, a Lean proof does not automatically establish
that its assumptions describe a real system or that
the theorem's informal explanation is accurate.

Mathematical correctness requires **correct formal definitions and proofs**,
**with assumptions and dependencies made explicit**.

### Criteria 2. Scientific Adequacy

A mathematically correct theory may still be
**inadequate for its intended applications**.
For example, an assumption might be satisfiable in a small formal model
but difficult to justify for actual public records or competing identity criteria.

Scientific adequacy requires clear connections
between formal concepts and the phenomena they represent,
supported by appropriate examples, evidence, or explicit limitations.

### Criteria 3. Theoretical Contribution

Correct mathematics and plausible models are not enough
to establish a substantive theoretical contribution.
The theory should **help with understanding** that was previously
unclear, unresolved, or insufficiently characterized.

Theoretical contribution requires an identifiable contribution,
appropriately situated relative to prior work,
with claims proportionate to the established results.
A contribution may be small, conditional, or limited in scope.

## Contributors

A doubt should be recorded when we identify a specific reason
that a research claim could be incorrect, inapplicable, insufficiently supported, or misunderstood.

### Status Values

| Status             | Meaning                                                                    |
| ------------------ | -------------------------------------------------------------------------- |
| **Open**           | A substantive question remains unanswered.                                 |
| **Open, check**    | An existing result may address the question, but has not been verified.    |
| **Resolved**       | The specific concern has been answered; the entry identifies the evidence. |
| **Standing rules** | Continuing safeguards against misinterpretation or overclaiming.           |

Resolving a doubt does not necessarily resolve every related scientific question.

### Recording a New Doubt

1. Identify the specific concern and the research criterion it affects.
2. Classify it as undermining, rebutting, or undercutting.
3. Assign the next available ID: `UM`, `RB`, or `UC`.
4. State the concern in ordinary language.
5. Explain what the current theory, evidence, or implementation establishes.
6. Identify what remains unresolved, or the documentation rule that prevents misinterpretation.

Preserve existing IDs so that references remain stable.

### Resolving a Doubt

When a concern is resolved:

- Change its status to `Resolved`.
- Explain exactly what established the resolution.
- Link or name the relevant theorem, model, experiment, or other evidence.
- Retain important scope limitations.

If a previously resolved doubt is reopened by new evidence, document why.

### Relationship to Other Repository Files

- **Lean source:** Formal definitions, assumptions, and mathematical proofs.
- **`reference/`:** Registered formal results and traceability information.
- **`DECISIONS.md`:** Design rationale, methodological choices, and proof boundaries.
- **`DOUBTS.md`:** Unresolved scientific questions, potential weaknesses, and safeguards against overclaiming.

## Terminology

The doubt categories come from argumentation theory:

- **Undermining:** Challenges a premise.
- **Rebutting:** Challenges a conclusion.
- **Undercutting:** Challenges the support connecting premises, results, and claims.

## References

See also:

- [Research vocabulary](docs/en/vocab.md)
- [Design decisions](DECISIONS.md)
- Prakken (2010), [An abstract framework for argumentation with structured arguments](https://doi.org/10.1080/19462160903564592)
- Pollock (1987), [Defeasible reasoning](https://doi.org/10.1207/s15516709cog1104_4)
- [Defeasible Reasoning](https://plato.stanford.edu/entries/reasoning-defeasible/), Stanford Encyclopedia of Philosophy
