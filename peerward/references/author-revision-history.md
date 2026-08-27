# Author Revision History Workflow

Use this workflow when a paper has meaningful Git or version history but no preserved reviewer comments or response letter.

## Evidence boundary

- A commit and manuscript diff can verify **when** a change occurred and **what** changed.
- They usually cannot verify **who requested** the change or the author's private motivation.
- Never rewrite an observed change as a reviewer concern without reviewer evidence.
- Label purpose statements as inferred and attach confidence: high when the change is coordinated across title, claims, method, and evidence; medium when the diff supports several plausible purposes; low when only a filename or terse commit message supports it.

## Build the revision chain

For each key node, record:

1. **Observed weakness before the change:** a mismatch, ambiguity, overclaim, proof defect, fragmented structure, or evidence gap visible in the earlier manuscript.
2. **Observed modification:** the exact claim, definition, theorem, section, experiment, or title that changed.
3. **Inferred scientific-writing purpose:** why the modification improves correctness, traceability, scope, or reader comprehension.
4. **Propagation check:** which downstream elements also needed updating.
5. **Resulting boundary:** what the revised paper can and still cannot claim.

Use the chain:

observed weakness → actual modification → inferred purpose [confidence] → validation/propagation → remaining limit

## Classify commits by scientific role

Prefer commits that change one or more of these:

- **Framing:** title, research question, motivation, novelty positioning, contribution hierarchy.
- **Formulation:** variables, assumptions, information access, objective, constraints, or problem boundaries.
- **Correctness:** theorem statements, proof steps, coefficients, inequalities, solution concepts, or parameter conditions.
- **Architecture:** merging or splitting sections to align problem, mechanism, and guarantee.
- **Evidence:** baselines, metrics, ablations, robustness settings, reproducibility information, or removal of redundant cases.
- **Scope:** weakening claims, removing umbrella language, narrowing applications, or adding limitations.

Treat formatting, generated files, build artifacts, and code churn as secondary unless they alter scientific communication.

## Select key version nodes

Choose a node when it marks a change in claim, problem formulation, proof framework, experiment role, title, or submission readiness. Do not select every commit. A useful history normally includes:

- earliest interpretable manuscript;
- each scientific turning point;
- explicit theorem/proof correction nodes;
- a major structural or evidence revision;
- the final or submitted-intent version, with status qualified by available evidence.

Repository-level line counts may be misleading when templates, figures, code, or generated files are tracked. Compare representative manuscript files and semantic sections.

## Propagation audits

Run the appropriate audit after a scientific change:

- **Definition or output semantics changed:** update algorithm, constraints, loss, theorem assumptions, metrics, abstract, and contributions.
- **Theorem or coefficient changed:** check upstream assumptions and parameter choices, then downstream corollaries, proofs, simulations, captions, and conclusions.
- **Claim strength changed:** update title, abstract, contribution list, related-work positioning, experiment language, and limitations.
- **Scope or example removed:** delete orphaned motivation, symbols, cross-references, figures, and unsupported generalizations.
- **Structure changed:** verify that each section has one role in the problem–mechanism–guarantee chain.

## Extract and promote lessons

A Git-derived lesson is initially a case-local hypothesis. Promote it to a shared Peerward principle only when at least two independent paper lineages show the same causal pattern. Record the supporting cases and evidence types privately; publish only the generalized principle and applicability boundary.

A theorem correction and a title rewrite within one lineage are multiple observations, not multiple independent cases.

