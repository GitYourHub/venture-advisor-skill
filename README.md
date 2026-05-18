# Mr-x-venture-advisor-skill

An opinionated venture advisor skill for Codex-style workflows.

This skill is designed for startup and new-project evaluation across both AI-native and traditional businesses. It focuses on evidence, stage discipline, and practical next steps instead of generic brainstorming.

## What it does

- Clarifies ambiguous project definitions with project-specific questions
- Distinguishes facts, assumptions, and unknowns
- Uses argument and counterargument structure instead of shallow pros and cons
- Prioritizes official and primary sources when market, policy, pricing, rules, or regulation matter
- Produces a decision-oriented assessment with clear stage gating

## Output style

Default analysis order:

1. `论证`
2. `反证式诊断`
3. `关键风险`
4. `重点评审结果`
5. `可行性结论`
6. `下一步行动`

## Included files

- `SKILL.md`
- `agents/openai.yaml`
- `references/founder-playbook.md`
- `references/engagement-patterns.md`
- `references/project-review-flow.md`

## Installation

Copy this repository into your Codex skills directory, for example:

```bash
cp -R venture-advisor-skill "$CODEX_HOME/skills/Mr-x-venture-advisor-skill"
```

Or create a symlink during local development:

```bash
ln -s /absolute/path/to/venture-advisor-skill "$CODEX_HOME/skills/Mr-x-venture-advisor-skill"
```

## Example prompt

```text
使用 $Mr-x-venture-advisor-skill 帮我判断这个创业项目现在处于什么阶段、主要风险是什么、下一步该做什么。
```

## Notes

- The skill asks clarification questions only when they materially affect judgment.
- Option lists are always numbered.
- AI-related questions are conditional, not mandatory.
