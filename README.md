# Justin's Skills

A curated collection of reusable, domain-agnostic skills for AI agents and automation workflows.

These skills are distilled from daily work experience, stripped of any company-specific business logic, and designed to be general-purpose building blocks that anyone can drop into their own projects.

## 📁 Repository Structure

```
.
├── skills/                     # Skill definitions and reference materials
│   └── <skill-name>/
│       ├── SKILL.md            # Skill specification and usage guide
│       └── references/         # Templates, patterns, and supporting docs
├── testcases/                  # Real-world usage examples for each skill
│   └── <skill-name>/
│       └── *.md                # Concrete examples and expected outputs
├── LICENSE
└── README.md
```

## ✨ Available Skills

### langgpt-prompt-generator

Generate structured, professional system prompts following the **LangGPT** specification. This skill helps you craft high-quality AI agent prompts that include role definition, skills, rules, workflow, and integrated few-shot examples.

**What it does**
- Provides a complete LangGPT template with standardized sections (`Role Definition`, `Profile`, `Skills`, `Rules`, `Workflow`, `Few-shot Examples`).
- Offers 5 ready-made few-shot patterns (`Q&A`, `Task Execution`, `Creative Generation`, `Code Generation`, `Analysis`) that you can adapt to your domain.
- Enforces quality checks (specific role, measurable skills, sequential workflow, edge-case coverage).

**When to use**
- Bootstrapping a new AI assistant or agent.
- Migrating an ad-hoc prompt into a maintainable, versioned format.
- Onboarding teammates to prompt-engineering best practices.

**Quick start**
1. Read the skill spec: [`skills/langgpt-prompt-generator/SKILL.md`](skills/langgpt-prompt-generator/SKILL.md)
2. Pick a pattern from [`references/few-shot-patterns.md`](skills/langgpt-prompt-generator/references/few-shot-patterns.md)
3. Fill in the template from [`references/langgpt-template.md`](skills/langgpt-prompt-generator/references/langgpt-template.md)
4. See concrete examples in [`testcases/langgpt-prompt-generator/`](testcases/langgpt-prompt-generator/)

## 🚀 Getting Started

Each skill is self-contained. To use one:

1. Navigate to the skill folder under `skills/`.
2. Read `SKILL.md` for the full specification and customization guidelines.
3. Check the corresponding `testcases/` folder for copy-pasteable examples.

No installation or dependencies required — these are plain Markdown specs meant to be consumed by humans and LLMs alike.

## 🤝 Contributing

Contributions are welcome! If you have a general-purpose skill you'd like to share:

1. Fork the repository.
2. Create a new folder under `skills/<your-skill-name>/` with a `SKILL.md` and any `references/`.
3. Add test cases under `testcases/<your-skill-name>/`.
4. Update this README with a short description of your skill.
5. Open a Pull Request.

Please keep skills domain-agnostic and free of proprietary business logic.

## 📄 License

[MIT](LICENSE)
