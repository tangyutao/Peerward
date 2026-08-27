# Evidence workflow for a paper case

## Inventory without mutation

List source, review, response, final, archive, and Git metadata. Detect LaTeX, BibTeX, PDF, DOCX, and plain-text files. Do not compile, normalize, rename, or rewrite source files during inventory.

Create the case index in the assistant project, not in the source directory. Prefer project-relative paths in `case.yaml`; record only evidence needed for the selected revision chain and leave unconfirmed roles as `needs_review`.

## Reconstruct chronology

Prefer Git commits, tags, and branches when they meaningfully track revision rounds. Otherwise infer chronology from round directories, filenames, review dates, response headings, and accepted or final folders. Mark file-based chronology as reconstructed rather than Git-derived.

Choose one representative manuscript and response per round. Record alternatives rather than silently discarding them. Verify titles and round assignments against document content; filenames and directory labels are navigation clues, not proof.

## Extract and verify evidence

Read reviewer reports and response letters. Build a coverage table with round, reviewer comment, author response, claimed location, verified manuscript change, and status. Use `verified`, `partial`, `response-only`, `not-found`, or `uncertain`. If review evidence is absent or only indirectly implied, state `unknown` rather than inferring reviewer intent.

Compare representative manuscripts semantically. Inspect framing, contributions, formulation, assumptions, information structure, theorem statements, solution concepts, proofs, gain conditions, implementability, module interfaces, experiments, baselines, metrics, limitations, and future-work boundaries. Line counts are navigation aids, not measures of scientific importance.

## Identify key nodes and decisions

A key version changes problem scope, novelty claim, mathematical model, proof framework, algorithm architecture, evidence type, or reviewer disposition.

For every major revision, write:

`Reviewer observation → latent acceptance risk → author strategy → verified change → why the change addresses the risk`

Create summaries only in the assistant project or another approved destination. Use project-relative or anonymized evidence paths in material intended for sharing.
