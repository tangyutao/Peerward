# Research question and argument design

Use this reference before drafting an outline, rewriting an introduction, or defending novelty.

## The research-value chain

Express the project as:

`topic → practical or theoretical situation → unresolved difficulty → research question → answer/claim → reasons or mechanism → evidence → limits → significance`

A topic is not yet a research problem. “Distributed optimization for nonlinear agents” names an area. A usable problem identifies what agents must achieve, what information and dynamics prevent existing solutions, and what guarantee is missing.

## Reader-need test

Answer four questions in reader order:

1. What does the community already know or do?
2. What important capability remains unavailable, unreliable, or unexplained?
3. Why does that limitation matter under the paper's intended conditions?
4. What does this paper establish that changes the reader's understanding or options?

Do not manufacture a gap by saying that something “has received little attention.” State the technical obstruction and its consequence.

## Claim map

For every major contribution, record:

| Element | Diagnostic question |
|---|---|
| Claim | What exactly is asserted? |
| Scope | For which systems, graphs, information structures, and initial conditions? |
| Mechanism | What new idea makes the result possible? |
| Reasons | Which intermediate facts connect the mechanism to the claim? |
| Evidence | Which theorem, proof, experiment, comparison, or case supports it? |
| Warrant | Why does that evidence justify this claim rather than a weaker one? |
| Limitation | What remains outside the result? |

If the evidence supports convergence only under weight-balanced graphs, the contribution must not imply arbitrary directed graphs.

## Novelty test

Compare the closest work along:

- problem and plant class;
- information available to each agent;
- assumptions and solution concept;
- technical obstruction;
- mechanism introduced;
- guarantee obtained;
- empirical or theoretical evidence.

Novelty is not a count of unfamiliar components. When familiar modules are composed, the contribution must identify the new compatibility problem, coupling analysis, regime, or guarantee.

## Contribution sentence pattern

Use this as a reasoning scaffold, not fixed prose:

`Under [conditions], we address [precise obstacle] by [mechanism], establish [guarantee], and validate [aspect] through [evidence].`

Remove adjectives such as “novel,” “effective,” and “significant” when the following clauses do not make them verifiable.

## Argument audit

Flag:

- claims without evidence;
- evidence not tied to a stated claim;
- assumptions introduced only inside proofs;
- comparison dimensions that favor one method unfairly;
- experiments that illustrate the theorem but do not test the paper's empirical claims;
- limitations hidden from the abstract, theorem, or conclusion.

