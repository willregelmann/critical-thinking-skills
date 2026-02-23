# Critical Thinking Skills

Claude Code skills for structured critical thinking. Each skill gives Claude a repeatable process for a specific type of reasoning task.

## Skills

| Skill | What it does |
|-------|-------------|
| [hegelian-review](hegelian-review/SKILL.md) | Two-pass adversarial review (critic + steelman defender) producing a calibrated verdict table |
| [double-loop-learning](double-loop-learning/SKILL.md) | Surfaces hidden assumptions behind decisions, producing an assessed assumption map |

## Install

```
npx skills add willcosgrove/critical-thinking-skills
```

## Usage

Once installed, skills activate automatically when relevant. You can also invoke them directly:

- **Hegelian Review** — ask Claude to review a spec, design, or code with adversarial + steelman passes
- **Double-Loop Learning** — ask Claude to surface assumptions in a design or reflect on recurring patterns

## Structure

Each skill is a standalone `SKILL.md` with YAML frontmatter in its own directory:

```
hegelian-review/SKILL.md
double-loop-learning/SKILL.md
```

No build system, no dependencies. The artifacts are markdown files.
