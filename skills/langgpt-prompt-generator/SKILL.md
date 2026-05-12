---
name: langgpt-prompt-generator
description: Generate LangGPT-style system prompts with few-shot examples. Use when you need to create structured, professional system prompts for AI agents that include role definition, constraints, workflow, and few-shot demonstrations. This skill provides templates and patterns for crafting high-quality system prompts following the LangGPT specification.
---

# LangGPT Prompt Generator

Generate structured system prompts following the LangGPT specification with integrated few-shot examples.

## LangGPT Structure

LangGPT prompts follow this structure:

```markdown
## Role Definition
[角色名称和核心目标]

## Profile
- Author: [作者]
- Version: [版本号]
- Language: [语言]
- Description: [简要描述]

## Skills
[技能1]
[技能2]
...

## Rules
[规则1]
[规则2]
...

## Workflow
1. [步骤1]
2. [步骤2]
...

## Few-shot Examples
[具体示例]
```

## Creating System Prompts

Follow this process:

1. **Understand the role** - Ask for clarification if the role or objectives are unclear
2. **Review templates** - See [langgpt-template.md](references/langgpt-template.md) for complete template
3. **Select few-shot pattern** - See [few-shot-patterns.md](references/few-shot-patterns.md) for example structures
4. **Generate the prompt** - Combine role definition with appropriate few-shot examples

## Customization Guidelines

- **Role Definition**: Clear, concise statement of the AI's purpose and domain
- **Skills**: 3-7 specific capabilities, written as bullet points
- **Rules**: 3-10 behavioral constraints, starting with strong verbs
- **Workflow**: Sequential steps (3-7) showing task completion process
- **Few-shot**: 2-4 representative examples showing input→output patterns

## Quality Checklist

- [ ] Role is specific and action-oriented
- [ ] Skills are distinct and measurable
- [ ] Rules address edge cases and constraints
- [ ] Workflow is logically sequential
- [ ] Few-shot examples cover common scenarios
- [ ] Language is consistent throughout
- [ ] No ambiguity in instructions
