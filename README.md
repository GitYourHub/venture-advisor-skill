# Mr-x-venture-advisor-skill

一个面向创业项目判断的顾问型技能，适用于 Codex 风格的工作流。

这个 skill 既适用于 AI 原生项目，也适用于传统服务、工具、渠道、内容和线下生意。它强调证据、阶段纪律和可执行动作，而不是泛泛而谈的灵感讨论。

这个 skill 基于 Anthropic 公司提出的《AI 原生创业者手册》相关方法论整理而成，仅用于学习交流。

## 这个 skill 能做什么

1. 当项目定义还模糊时，用贴着项目本身的问题做澄清
2. 区分已验证事实、关键假设和未知项
3. 用“论证 + 反证式诊断”的方式做项目判断，而不是简单列优缺点
4. 在涉及市场、政策、定价、规则、监管时，优先使用官方和一手资料
5. 输出面向决策的结论，明确当前阶段能不能继续往下走

## 默认输出顺序

1. `论证`
2. `反证式诊断`
3. `关键风险`
4. `重点评审结果`
5. `可行性结论`
6. `下一步行动`

## 仓库内容

- `SKILL.md`
- `agents/openai.yaml`
- `references/founder-playbook.md`
- `references/engagement-patterns.md`
- `references/project-review-flow.md`

## 安装方式

把这个仓库复制到你的 Codex skills 目录，例如：

```bash
cp -R venture-advisor-skill "$CODEX_HOME/skills/Mr-x-venture-advisor-skill"
```

如果你在本地迭代开发，也可以用软链接：

```bash
ln -s /绝对路径/venture-advisor-skill "$CODEX_HOME/skills/Mr-x-venture-advisor-skill"
```

## 使用示例

```text
使用 $Mr-x-venture-advisor-skill 帮我判断这个创业项目现在处于什么阶段、主要风险是什么、下一步该做什么。
```

## 说明

1. 只有当澄清问题会显著影响判断时，skill 才会继续追问
2. 只要出现选项，选项必须带连续序号
3. AI 相关问题不是默认必问，只有在确实影响判断时才问
