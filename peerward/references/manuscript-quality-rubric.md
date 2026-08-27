# Manuscript Quality Rubric

Use this reference for pre-submission quality assessment, supervisor-style manuscript diagnosis, or comparison of versions. The score is an evidence-indexed diagnostic, not an acceptance probability.

## Gate checks

Before scoring, identify any critical blocker:

- unsupported or internally contradictory central claim;
- invalid or uncheckable theorem/proof dependency;
- ill-posed formulation or unavailable information in an alleged distributed method;
- fabricated, missing, or mismatched evidence;
- unverified citation presented as fact;
- ethical, authorship, confidentiality, or data-integrity concern.

A manuscript with an unresolved critical blocker is **not submission-ready**, regardless of its numerical score.

## Scoring method

Score each dimension from 0 to 4. Its weighted contribution is `(score / 4) × weight`:

- 0: absent, contradictory, or not assessable;
- 1: fundamental deficiency;
- 2: plausible but incomplete;
- 3: sound with material improvements still possible;
- 4: clear, rigorous, and proportionate to the paper's scope.

Every score requires:

location/evidence → judgment → consequence → minimum action → verification

Use not-assessed rather than guessing. If a dimension is genuinely inapplicable, explain the redistribution before calculating a total.

## Default 100-point profile

| Dimension | Weight | Core question |
|---|---:|---|
| Research question and significance | 10 | Is there a clear reader need and consequential problem? |
| Novelty and contribution | 15 | Is the new obstruction, mechanism, capability, or guarantee distinguishable from the closest baseline? |
| Formulation and assumptions | 15 | Are objects, information, objectives, constraints, and applicability boundaries precise? |
| Method or algorithm explanation | 10 | Can a qualified reader understand and implement the method? |
| Theory and correctness | 15 | Do definitions, theorem statements, proof logic, and parameter conditions support the claims? |
| Experiments and comparisons | 15 | Do baselines, metrics, settings, and analyses test the stated claims? |
| Reproducibility and transparency | 5 | Is there enough information to reproduce or independently check the work? |
| Argument and paper architecture | 7 | Does the paper follow a problem–mechanism–guarantee–evidence chain? |
| Mathematical exposition | 4 | Are notation, equations, and proof navigation readable and consistent? |
| Language and presentation | 4 | Is the text clear enough that language does not hide the science? |

## Interpretation

- **85–100, Ready with checks:** no critical blocker; only bounded revisions remain.
- **70–84, Major internal revision:** core work is plausible, but one or more high-risk dimensions are not yet convincing.
- **55–69, Fundamental revision:** contribution or evidence chain requires restructuring.
- **Below 55, Not ready:** the manuscript cannot yet support a credible submission decision.

Do not use the label accept or reject. Assess venue fit separately from intrinsic manuscript quality.

## Paper-type adaptation

- For theory-heavy papers, increase theory/correctness and reduce empirical weight only after requiring an appropriate numerical or explanatory validation role.
- For empirical AI papers, increase experiments, reproducibility, data, and statistical analysis.
- For review papers, replace method performance with search strategy, inclusion criteria, synthesis quality, coverage, and bias assessment.
- For short letters, do not lower rigor; reduce expected breadth and require a sharper single contribution chain.

## Required output

Return:

1. gate-check result;
2. dimension table with score, evidence, confidence, and action;
3. total only over assessed dimensions;
4. top three submission risks;
5. minimum path to the next readiness band;
6. claims that must be narrowed if no new evidence is added;
7. limitations of the assessment.

## Calibration rule

When comparing versions, score both against the same rubric and explain what evidence changed. A higher-quality rewrite without new proof or experiment must not increase correctness or evidence scores merely because it reads better.
