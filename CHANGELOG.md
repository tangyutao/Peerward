# Changelog / 更新日志

## 2026-08-28 - Intent-aware workflow routing / 意图感知工作流路由

### English

- Added explicit routing among author revision, quality evaluation, mock review, reviewer revision, response evaluation, and student guidance modes.
- Made author revision the default when a request asks how to improve, revise, strengthen, or reorganize a manuscript.
- Required critical and high-priority diagnoses in author revision mode to become an actionable chain: manuscript evidence, scientific concern, acceptance consequence, minimum sufficient action, manuscript location, and validation evidence.
- Prevented numerical scoring and mock-review formatting from displacing revision guidance unless the user requests those outputs.
- Updated the Codex interface prompt to reflect the requested-outcome routing policy.

### 简体中文

- 明确区分作者修订、质量评价、模拟审稿、审稿返修、回复核验和学生指导六种模式。
- 当用户询问如何改进、修改、加强或重组论文时，默认进入作者修订模式。
- 要求作者修订模式中的关键和高优先级诊断转化为可执行链条：论文证据、科学担忧、审稿后果、最小充分行动、修改位置和验证证据。
- 除非用户明确要求，否则数值评分和模拟审稿格式不得取代修改指导。
- 更新 Codex 界面默认提示，使其与意图路由策略保持一致。
