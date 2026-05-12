# LangGPT Prompt Template

## Complete Template Structure

```markdown
## Role Definition

[AI助手名称] - [一句话核心目标描述]

## Profile

- Author: [作者名称]
- Version: [版本号，如 1.0]
- Language: [语言，如 中文/English]
- Description: [2-3句话描述助手的专业领域和主要功能]

## Skills

1. [技能名称] - [简要描述该技能的作用]
2. [技能名称] - [简要描述该技能的作用]
3. [技能名称] - [简要描述该技能的作用]
4. [技能名称] - [简要描述该技能的作用]
5. [技能名称] - [简要描述该技能的作用]

## Rules

1. [行为规则] - 始终[具体行为要求]
2. [行为规则] - 必须[具体行为要求]
3. [行为规则] - 禁止[具体行为要求]
4. [行为规则] - 当[条件]时，应该[行为]
5. [行为规则] - 优先[排序原则]
6. [行为规则] - 避免[常见错误]
7. [行为规则] - 保持[质量标准]

## Workflow

1. [步骤一]：[具体操作，包含判断条件和处理方式]
2. [步骤二]：[具体操作，与前一步的逻辑关系]
3. [步骤三]：[具体操作，完成标准]
4. [步骤四]：[具体操作，输出格式要求]
5. [步骤五]：[具体操作，验证和确认]

## Few-shot Examples

### Example 1
User: [用户输入]
Assistant: [期望输出]

### Example 2
User: [用户输入]
Assistant: [期望输出]

### Example 3
User: [用户输入]
Assistant: [期望输出]
```

## Section Guidelines

### Role Definition
- **Length**: 1-2 sentences
- **Content**: Name + core purpose
- **Style**: Professional, concise

### Profile
- **Author**: Creator or organization
- **Version**: Semantic versioning (1.0, 1.1, 2.0)
- **Language**: Target language of the prompt
- **Description**: Domain + main capabilities

### Skills
- **Quantity**: 3-7 skills
- **Format**: `[Action verb] + [object] + [optional qualifier]`
- **Examples**:
  - "Analyze complex data patterns and identify trends"
  - "Generate code snippets in multiple programming languages"
  - "Translate technical concepts for non-technical audiences"

### Rules
- **Quantity**: 3-10 rules
- **Format**: `[Strong verb] + [specific requirement]`
- **Verb examples**: Always, Must, Never, When, Prioritize, Avoid, Ensure
- **Examples**:
  - "Always provide source citations for factual claims"
  - "Never assume user context beyond the conversation"
  - "When multiple approaches exist, recommend the simplest one"

### Workflow
- **Quantity**: 3-7 steps
- **Format**: `Step [N]: [Action verb] + [what/how]`
- **Flow**: Sequential and logical
- **Examples**:
  - "Step 1: Analyze the user's request to identify the core task"
  - "Step 2: Retrieve relevant information from provided context"
  - "Step 3: Generate a structured response addressing the query"

### Few-shot Examples
- **Quantity**: 2-4 examples
- **Purpose**: Demonstrate input-output patterns
- **Selection**: Common, representative scenarios
- **Format**: Clear demarcation between User and Assistant
