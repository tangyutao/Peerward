# Peerward v1.0.0

Peerward's first public release provides an evidence-based research-writing workflow that guides a manuscript from research results toward supervisor and peer review. It focuses on the scientific reason for each revision—not just sentence-level polishing—and keeps recommendations traceable to manuscript evidence and validation criteria.

## Highlights

- **Intent-aware workflow routing:** distinguishes author revision, quality evaluation, mock review, reviewer revision, response evaluation, and student guidance, with actionable author-side revision as the default when the goal is to improve a manuscript.
- **Traceable revision decisions:** turns important diagnoses into a chain from manuscript evidence and scientific concern to the minimum sufficient action, target location, and validation evidence.
- **Full-paper scientific guidance:** supports research-question and contribution design, paper architecture, mathematical definitions and proofs, experiments and comparisons, and scientific English.
- **Reviewer-response verification:** connects reviewer concerns, revision strategy, actual manuscript changes, and response-letter claims instead of treating promised changes as completed work.
- **Evidence-aware evaluation:** provides submission-readiness assessment and clearly labeled mock review when requested, while reporting missing evidence and avoiding invented claims, results, references, or reviewer intent.
- **Teaching and reproducibility resources:** includes bilingual prompt libraries, structured output schemas, multi-round mentoring guidance, Git-history analysis, and a fully synthetic example case.
- **Privacy and responsible-use safeguards:** excludes real confidential review material and documents boundaries for authorship, AI disclosure, official peer review, scoring, and human accountability.

## Included resources

- English and Simplified Chinese documentation and prompt libraries
- 15 focused reference guides for research writing, mathematical exposition, evaluation, revision, and mentoring
- Codex agent interface configuration
- Synthetic manuscript/reviewer example with an expected analysis
- MIT License

## Installation

Copy the `peerward` directory into your Codex skills directory, then invoke it with a request such as:

```text
$peerward diagnose the scientific and mathematical weaknesses in this manuscript and prioritize actionable revisions.
```

See [README.md](README.md), [README.zh-CN.md](README.zh-CN.md), and the bilingual prompt libraries for complete usage examples.

---

Peerward 的首个公开版本提供了一套证据驱动的科研论文写作与修订工作流，帮助作者将研究结果逐步组织为可接受导师审阅和同行评审的论文。它关注每项修改背后的科学理由，而不仅是句子润色，并将建议与论文证据和验证标准对应起来。

## 主要特性

- **意图感知工作流路由：** 区分作者修订、质量评价、模拟审稿、审稿返修、回复核验和学生指导六种模式；当目标是改进论文时，默认提供可执行的作者侧修订建议。
- **可追溯的修订决策：** 将重要诊断转化为从论文证据、科学担忧到最小充分行动、修改位置和验证证据的完整链条。
- **全流程科学写作指导：** 覆盖研究问题与贡献设计、论文结构、数学定义与证明、实验与对比，以及科研英语。
- **审稿回复核验：** 关联审稿意见、修订策略、正文实际修改与回复信主张，不把回复中的承诺直接视为已完成修改。
- **证据约束的质量评价：** 按需提供投稿就绪度评估和明确标注的模拟审稿；证据不足时报告未知项，不虚构结论、结果、参考文献或审稿人意图。
- **教学与复现资源：** 提供中英文提示词库、结构化输出规范、多轮指导流程、Git 历史分析方法和完整的合成案例。
- **隐私与负责任使用边界：** 不包含真实保密审稿材料，并明确作者责任、AI 使用披露、正式同行评审、评分与人工问责边界。

## 安装

将 `peerward` 目录复制到 Codex 的 skills 目录，然后使用类似以下的请求调用：

```text
$peerward 诊断这篇论文在科学论证与数学表达方面的问题，并按优先级给出可执行的修改方案。
```

完整用法请参阅 [README.md](README.md)、[README.zh-CN.md](README.zh-CN.md) 和中英文提示词库。
