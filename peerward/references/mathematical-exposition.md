# Mathematical exposition

Use this reference for notation, definitions, assumptions, theorem statements, equations, and proofs.

## Symbol lifecycle audit

For every symbol, verify:

1. it is defined before or immediately after first use;
2. its type, dimension, domain, and dependencies are recoverable;
3. it is not reused for a different object;
4. the reader knows whether it is local, global, measured, estimated, or designed;
5. it remains necessary often enough to justify notation;
6. its role does not silently change between theorem, proof, and simulation.

Prefer mnemonic labels and descriptive names over dense indices. Introduce shorthand only when it reduces repeated cognitive load.

## Definition audit

A definition should make membership testable. Check:

- object being defined;
- ambient set or system;
- required properties and quantifiers;
- dependence on earlier definitions;
- boundary cases;
- one example or counterexample when the concept is nonstandard.

Do not define a property only because a theorem needs a short statement. Explain why the property captures the technical obstacle.

## Theorem contract

Read every theorem as a contract:

| Contract element | Question |
|---|---|
| Object | What system, algorithm, or solution is covered? |
| Conditions | Which assumptions, graph properties, gains, and initial states are required? |
| Information | Are all controller inputs available under the stated architecture? |
| Guarantee | Existence, boundedness, convergence, rate, optimality, robustness, or parameter recovery? |
| Quantifiers | What is uniform, local, global, or dependent on a parameter? |
| Solution concept | Classical, Carathéodory, Filippov, weak, stochastic, or another notion? |

Keep consequences and interpretation outside the formal statement. Use “an optimal solution” unless uniqueness has been established.

## Proof architecture

Before details, provide a proof map when the argument is long:

`Step 1 establishes well-posedness → Step 2 bounds internal states → Step 3 proves convergence of the coordination signal → Step 4 transfers convergence to physical outputs.`

Then audit:

- every step has stated inputs and output;
- forward dependencies are visible;
- motivation, heuristic explanation, and rigorous argument are distinguishable;
- skipped steps are truly standard and have a hint or citation;
- assumptions are used explicitly;
- difficult algebra is separated from the conceptual reason it works;
- the conclusion matches the theorem's quantifiers and scope.

Avoid “clearly,” “obviously,” and “it is easy to see” when they replace reasoning. Replace them with the missing fact, lemma, or one-line argument.

## Equation-as-sentence rule

Mathematical displays participate in grammar. Introduce them, punctuate them consistently, and explain what changes after them. Do not start a sentence with a bare symbol. Keep causal order linear: fact → invoked result → consequence.

## Assumption stress test

For each important assumption, state:

- where it enters the proof;
- what breaks without it;
- whether it is structural, technical, or chosen for exposition;
- whether an example or counterexample demonstrates necessity;
- how it compares with assumptions in the closest work.

