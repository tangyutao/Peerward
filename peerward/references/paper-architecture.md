# Paper architecture

Use this reference to design or diagnose the whole manuscript. Treat the structure as a functional map, not a rigid template.

## Reader path

A technical paper should let a reader recover, in this order:

1. the problem and why it matters;
2. the closest existing capability and the unresolved obstacle;
3. the exact model, information, assumptions, and objective;
4. the main result before long technical detail;
5. the mechanism and proof logic;
6. the meaning, evidence, limitations, and consequences.

Move material when its current location forces the reader to use a concept before understanding why it exists.

## Section function map

| Section | Primary job | Failure signal |
|---|---|---|
| Title | Make the searchable subject and result class identifiable | clever but non-searchable wording; broader scope than the theorem |
| Abstract | State problem, main result, distinguishing condition/mechanism, and evidence or implication | motivation-only opening; equations, citations, undefined abbreviations; no result |
| Introduction | Build problem–literature–gap–contribution logic | citation catalogue; generic importance; contributions detached from gaps |
| Related work | Compare the closest approaches on decision-relevant dimensions | chronological list without technical comparison |
| Problem formulation | Define system, actuation, sensing/information, assumptions, and objective | global variables used by local agents; hidden quantifiers; undefined solution concept |
| Main result | State the strongest clean guarantee early | main theorem delayed behind auxiliary lemmas; consequences mixed into theorem statement |
| Method/algorithm | Make the mechanism and implementation traceable | update law uses unavailable signals; tuning rules appear only in proofs |
| Proof | Make the logical route inspectable | backward jumps, unexplained cancellations, “obvious” steps, mixed motivation and rigor |
| Experiments | Test a claim, mechanism, robustness property, or practical interpretation | decorative trajectory plots; mismatched baselines; selected single run |
| Conclusion | Consolidate meaning, limits, and credible next questions | abstract repeated verbatim; new claims; vague future work |

## Architecture checks

- State the main result before readers encounter a long proof apparatus.
- Put definitions close to first meaningful use unless a small global notation block materially reduces repetition.
- Keep the main text logically self-contained even when proofs move to appendices. State any invoked lemma in the main text.
- Use diagrams to expose information and module interfaces, not to decorate the paper.
- Give each paragraph one controlling purpose; paragraph order should follow the argument, not the order in which research was performed.

## Control-paper backbone

For control and multi-agent work, the formulation should normally expose:

`plant/process → controlled input → disturbances/uncertainty → measured output → communication/information structure → controller/algorithm objective → guarantee`

This backbone prevents a frequent failure: presenting dynamics and an algorithm while leaving unclear who knows which variables and what “distributed” means operationally.

