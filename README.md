# Peerward

[English](README.md) | [简体中文](README.zh-CN.md)

Copy-ready workflows: [Prompt Library](PROMPTS.md) | [中文提示词库](PROMPTS.zh-CN.md) | [Changelog](CHANGELOG.md)

**Guide every draft toward peer review.**

Peerward is an evidence-based AI research-writing mentor for the full lifecycle of a scientific paper. It guides students from research results to a first draft, improves scientific arguments and mathematical exposition, evaluates manuscript quality, generates professional mock reviews, plans reviewer-driven revisions, and verifies response-letter quality.

The name combines *peer* with the directional suffix *-ward*: the system helps move each draft toward the standard expected in supervisor and peer review without claiming to guarantee correctness or acceptance.

It is designed for research in control, optimization, multi-agent systems, autonomous systems, and AI for control. The Skill focuses on why a revision is needed, not merely how a sentence should be polished.

## Latest update

Peerward now routes requests by the user's intended outcome. Requests asking how to improve a manuscript default to actionable **author revision** guidance; quality scoring and mock-review formats are used when requested. Critical and high-priority diagnoses are converted into a traceable chain from manuscript evidence to revision action and validation. See the [Changelog](CHANGELOG.md).

## Install

Copy the `peerward` directory into your Codex skills directory, then invoke it with:

```text
$peerward analyze these reviewer comments and the related manuscript section.
```

You can provide research notes, manuscript sections, reviewer comments, response letters, Git history, or versioned LaTeX files. Peerward can help structure a paper from scratch or diagnose an existing one. Missing evidence is reported rather than invented.

If reviewer comments or a response letter are unavailable, Peerward can still reconstruct author-side revision decisions from Git and manuscript diffs. It reports observed changes separately from inferred purposes and never invents reviewer causality.

## Knowledge modes

- supervisor-style first-draft guidance and multi-round mentoring;
- research question and argument design;
- paper and section architecture;
- mathematical definitions, notation, theorem statements, and proofs;
- scientific English for multilingual authors;
- evidence-indexed manuscript quality evaluation;
- professional mock peer review;
- reviewer-driven revision and verified response strategy.

These capabilities are routed as distinct operating modes: author revision, quality evaluation, mock review, reviewer revision, response evaluation, and student guidance.

The writing guidance is an original synthesis of established research-writing and mathematical-writing sources. Source titles are recorded for provenance, but copyrighted textbook text is not included.

## How to use the method

Invoke `$peerward` and provide the available evidence together with the decision you need to make. Useful inputs include a research question, manuscript section, LaTeX source, reviewer comments, response letter, or Git revision range. Keep confidential material in your local workspace; do not paste it into public issues or commits.

Peerward analyzes a paper in this order:

1. research question and reader need;
2. claim, reasons, evidence, assumptions, and limitations;
3. paper and section architecture;
4. mathematical definitions, notation, theorems, and proofs;
5. paragraph flow and sentence-level English;
6. reviewer concern, revision action, validation evidence, and response strategy.

The method records the causal chain

```text
reviewer comment → underlying concern → revision strategy
→ actual or proposed modification → validation evidence → transferable lesson
```

It therefore explains **why** a change is needed instead of merely reporting that text, theory, or experiments were added.

### Example prompts

For complete project-context, paper-design, reviewer-response, Git-history, mathematical-audit, privacy-audit, and GitHub-maintenance prompts, see the [Prompt Library](PROMPTS.md).

Plan a paper before drafting:

```text
$peerward turn these research notes into a claim map and paper outline.
```

Revise a manuscript section:

```text
$peerward diagnose the scientific and mathematical weaknesses in this introduction and theorem section. Prioritize structural issues before language polishing.
```

Respond to reviewers:

```text
$peerward analyze these reviewer comments with the related manuscript and response letter. For each concern, recommend a revision, decide whether theory or experiments are needed, and draft a response strategy.
```

Learn from revision history:

```text
$peerward compare these LaTeX revisions or Git commits, identify the key scientific-writing decisions, and extract 3–10 transferable lessons.
```

Expected outputs may include a claim map, revision priorities, section-level actions, theory/experiment/comparison judgments, response-letter guidance, evidence gaps, and a `case_summary.md` when case-level evidence is available.

## Student use

Start with the synthetic example in `examples/synthetic-case/`. It contains no real manuscript, author, reviewer, institution, submission identifier, or confidential review material.

## Privacy boundary

This repository contains only generalized workflow rules and synthetic teaching data. Do not commit unpublished manuscripts, real reviewer reports, response letters, submission IDs, personal data, local absolute paths, API credentials, or private Git history. See [PRIVACY.md](PRIVACY.md).

For authorship, confidential peer review, AI-use disclosure, scoring limits, and human accountability, see [RESPONSIBLE_USE.md](RESPONSIBLE_USE.md).

## License

MIT License. See [LICENSE](LICENSE).
