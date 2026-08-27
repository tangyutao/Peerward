# Reviewer concern strategies

| Category | Likely underlying risk | Minimum useful strategy |
|---|---|---|
| Novelty | The delta from closest work is not consequential | Compare condition, mechanism, guarantee, information assumption, and evidence; narrow the claim if components are known |
| Motivation | The problem lacks a credible use or gap | Connect the mathematical obstacle to an application constraint |
| Problem formulation | Variables, objectives, information, or scope are inconsistent | Restate objective, local data, communication, constraints, equilibrium, and implementability coherently |
| Assumption | The theorem relies on unrealistic or hidden structure | Explain where each assumption enters, what fails without it, and whether it is structural or removable |
| Theoretical proof | Correctness, well-posedness, or convergence is unsupported | Repair definitions and proof tools; add lemmas or restrict the claim |
| Algorithm explanation | The method cannot be implemented or modules are opaque | Provide update rules, signals, interfaces, and gain selection |
| Comparison | Advantage over relevant work is unverified or unfair | Align assumptions and information, use closest baselines, and report comparable metrics |
| Simulation | Claims lack stress, isolation, or practical meaning | Choose robustness, ablation, mechanism, or application tests according to the doubt |
| Writing clarity | Readers cannot recover the logic or notation | Repair the problem–gap–method–guarantee chain before polishing sentences |
| Contribution statement | Claims are broad or describe ingredients | State condition removed, mechanism introduced, guarantee obtained, and evidence supplied |

Add theory for correctness and convergence; experiments for effectiveness and robustness; comparison for relative advantage; explanation only when existing evidence already answers the concern.

A strong response contains acknowledgment, interpretation, concrete action, exact location, and resolution logic.

## Cross-case lessons

Treat a lesson from one paper as a case-local hypothesis. Promote it into this shared section only after at least two independent paper cases support the same `trigger → action → rationale → outcome` pattern with direct evidence. Different submissions or venue branches of the same underlying manuscript count as one case lineage, not independent confirmation. Track support counts and source cases privately; retain only the generalized rule and its boundary in public files.

- If an application claim has no model mapping or evidence, narrow it to the properties actually proved.
- When novelty is challenged, state the inherited baseline, new technical obstruction, resolving mechanism, and uncovered scope separately.
- For global graph quantities or planning inputs, disclose who knows them, how they are obtained, and the performance or implementation cost.
- For a proof correction, identify the faulty step and show the replacement derivation; a response-letter promise alone is `response-only`.
- Give every experiment or example one explicit purpose and matching metric; qualitative plots do not establish resource savings or superiority by themselves.
