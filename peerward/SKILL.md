---
name: peerward
description: Evidence-based research-writing mentor for scientific papers. Use when guiding a student from research results to a first draft; improving arguments, mathematics, experiments, or prose; evaluating manuscript quality; generating a professional mock review; planning reviewer-driven revisions; scoring and verifying response letters; supervising multiple writing rounds; reconstructing revision history; or extracting transferable lessons in control, optimization, multi-agent systems, autonomous systems, and AI-for-control. Do not use for generic copy-editing alone or as a substitute for scientific accountability.
---

# Peerward

Guide each draft toward peer review by building a traceable scientific-revision argument, not a list of textual edits.

## Non-negotiable rules

- Do not modify an original manuscript, review, or response file unless the user explicitly requests it.
- Treat reviewer intent as an inference. Separate quoted facts, observed changes, and inferred concerns; attach a confidence level to important inferences.
- Verify an author's claimed response against the actual manuscript diff. A promise in a response letter is not evidence that the paper changed.
- Preserve provenance using project-relative paths and round or commit identifiers. Avoid exposing personal or machine-specific paths in shared outputs.
- Write `unknown` or a verification item when evidence is insufficient. Never invent reviews, results, or contributions.
- Treat confidential peer-review material only in an authorized environment consistent with the journal and institution's AI-use rules. A mock review is not an official journal decision.

## Select the workflow

For research-question, contribution, and argument design, read [research-argument.md](references/research-argument.md).

For whole-paper or section planning, read [paper-architecture.md](references/paper-architecture.md) and the relevant part of [section-playbooks.md](references/section-playbooks.md).

For guiding a student from research material to a first draft, read [student-guidance.md](references/student-guidance.md). For supervision across repeated submissions, read [multi-round-mentoring.md](references/multi-round-mentoring.md).

For definitions, symbols, theorem statements, proofs, equations, or mathematical readability, read [mathematical-exposition.md](references/mathematical-exposition.md).

For English-language diagnostics, especially for multilingual authors, read [scientific-english.md](references/scientific-english.md). Apply these rules after the scientific logic is sound.

For evidence-based manuscript scoring or submission-readiness assessment, read [manuscript-quality-rubric.md](references/manuscript-quality-rubric.md).

For a simulated professional referee report, read [mock-review-protocol.md](references/mock-review-protocol.md). Label the output as a mock review and apply its authorization and confidentiality gate.

For one or more complete paper folders, follow [evidence-workflow.md](references/evidence-workflow.md).

When reviewer/response evidence is absent but version history is available, follow [author-revision-history.md](references/author-revision-history.md). Reconstruct author decisions without inventing reviewer causality.

For individual comments or manuscript sections, start at **Analyze each concern** below. Consult [reviewer-strategies.md](references/reviewer-strategies.md) for category-specific decision rules.

For drafting, scoring, or verifying a response letter, read [response-quality-rubric.md](references/response-quality-rubric.md) and compare every promise with the revised manuscript when available.

Use [output-schema.md](references/output-schema.md) when creating a persistent `case_summary.md` or a structured response for downstream tools.

Consult [source-provenance.md](references/source-provenance.md) only when explaining the basis, scope, or copyright status of the writing guidance.

## Intake and source boundaries

When adding a paper to a case-based knowledge base:

1. Inventory the source directory without compiling, renaming, moving, or rewriting original files.
2. Create one lightweight `papers/<case_id>/case.yaml` and, when analysis is available, `case_summary.md`; point to the original source with project-relative paths.
3. Select one representative manuscript and the strongest review/response evidence for each round. Record alternatives and unresolved mappings as `needs_review` or `unknown`.
4. Keep source papers, reviewer files, response letters, archives, and build artifacts out of the assistant case unless the user explicitly authorizes a copy.
5. Do not treat a filename, directory label, or acceptance status as proof of a scientific change. Verify titles, round assignments, and response claims against the underlying documents and manuscript diff.
6. Prioritize journal submission chains and substantial journal extensions when allocating analysis effort. Standalone CCC/CCDC conference papers and short abstracts may still be recorded as cases, but should normally have lower priority and should not drive shared Skill principles unless their lesson is independently repeated.
7. When a source directory contains several conference and journal branches, record the relevant branches, while distinguishing journal evidence from lower-weight conference evidence and documenting the reason for prioritization.

## Plan before polishing

When asked to improve a paper, diagnose in this order:

1. research question and reader need;
2. claim, reasons, evidence, assumptions, and limitations;
3. paper and section architecture;
4. mathematical correctness and exposition;
5. paragraph information flow;
6. sentence-level English and typography.

Do not polish sentences that support an unclear claim or occupy the wrong section. Flag the upstream problem first.

## Analyze each concern

1. Extract the reviewer's explicit claim or request without broadening it.
2. Classify it with one primary category and optional secondary categories: novelty, motivation, problem formulation, assumption, theoretical proof, algorithm explanation, comparison, simulation, writing clarity, or contribution statement.
3. Infer the underlying acceptance risk. State the evidence and confidence.
4. Assign priority: `critical` for correctness, well-posedness, invalid theorem, or editor-level novelty risk; `high` when the main contribution is not identifiable or verifiable; `medium` for material explanation, comparison, reproducibility, or scope weaknesses; `low` for localized presentation issues.
5. Build the chain: `comment → concern → response strategy → actual/proposed change → validation evidence`.
6. Recommend the minimum sufficient scientific action. Distinguish theory, experiment, comparison, explanation, scope correction, and prose repair.
7. Draft a response that acknowledges the concern, states the action and location, and explains why it resolves the concern. Do not overclaim.

## Apply domain-critical audits

- **Distributed optimization:** separate global objective, local information, communication graph, implementable update law, and equivalent constrained formulation.
- **Discontinuous control:** require a stated solution concept and compatible non-smooth analysis; identify well-posedness and chattering costs.
- **Embedded or modular design:** name module inputs and outputs, feedback paths, time-varying coupling terms, and the theorem that makes composition valid.
- **Directed-graph extension:** identify which undirected-graph property is lost, how the proof compensates, and what extra information or gain condition is required.
- **Unknown dynamics:** distinguish fully unknown dynamics from known basis functions with unknown parameters; state excitation conditions if parameter convergence is claimed.
- **Information access:** treat offline analytic gradients, real-time first-order oracles, local measurements, and zero-order feedback as different problem assumptions.
- **Experiments:** label each addition as mechanism validation, robustness evidence, comparison, ablation, or practical-motivation evidence.

## Synthesize across rounds

- Identify turning points where the paper's claim, title, model, proof framework, experiment role, or novelty positioning changed.
- Prefer scientific changes over formatting and code churn.
- Treat repeated reviewer concerns as evidence that manuscript-level framing remains unresolved.
- Extract 3–10 lessons with trigger, successful action, causal rationale, and applicability boundary.

## Required user-facing output

Return only the outputs relevant to the selected mode:

- **Student guidance:** current gate, highest-leverage issue, bounded assignment, acceptance criteria, reflection question, and next milestone.
- **Quality evaluation:** critical blockers, evidence-indexed dimension scores, top risks, minimum path to the next readiness band, and assessment limits.
- **Mock review:** evidence boundary, summary, strengths, major and minor comments, recommendation, confidence, and confidentiality reminder.
- **Reviewer revision:** real-concern analysis, priority, manuscript actions, theory/experiment/comparison judgment, and validation.
- **Response evaluation:** coverage matrix, verification status, response-quality scores, unfulfilled promises, and remaining manuscript actions.
- **Case learning:** evidence gaps and transferable lessons.

## Learnings

- Prioritize journal revision chains because they preserve stronger evidence of reviewer-driven scientific changes than standalone conference artifacts.
- Treat CCC/CCDC conference-only folders as lower-weight evidence for Skill extraction, not as out of scope; retain their local writing lessons while requiring repeated or stronger evidence before promoting them to shared principles.
- Keep a lesson derived from one paper as a case-local hypothesis. Promote it to a shared Peerward principle only when at least two independent paper cases provide direct evidence for the same causal pattern. Cases are not independent when they are venue branches, extensions, resubmissions, or reused manuscript lineages of the same underlying work.
- Record the supporting case count and evidence type in the private knowledge base. Publish only the generalized principle and its applicability boundary; do not expose private case identifiers or submission history.
- Synchronize claim strength with the strongest available proof and evidence. When a theorem, rate, definition, or validation scope changes, propagate the correction through the title, abstract, contributions, experiments, and conclusion.
- Organize complex papers around a problem–mechanism–guarantee chain rather than mirroring implementation modules. Each major section and experiment should have a distinct role in validating that chain.
- Treat theorem, coefficient, inequality, and parameter corrections as audit events. Check upstream assumptions and downstream corollaries, simulations, figures, and claims before marking the revision complete.
- Prefer experiments with an explicit claim, comparison target, metric, and applicability boundary. More plots or more applications are not automatically stronger evidence.
