# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A collection of Claude Code skills for structured critical thinking. Each skill is a standalone SKILL.md file in its own directory, installable via `npx skills add <owner>/critical-thinking-skills`.

## Repository Structure

```
<skill-name>/SKILL.md    — one directory per skill, one file per skill
```

There is no build system, no tests, no dependencies. The artifacts are markdown files with YAML frontmatter.

## Skill Format

Every SKILL.md must have:
- YAML frontmatter with `name` (lowercase, hyphens) and `description` (single line explaining what it does and when to use it)
- A structured process section with numbered steps
- A quick reference table summarizing the steps
- Common mistakes section (what goes wrong when the skill is misapplied)
- Key principles section (the non-obvious insights that make it work)

## Writing Conventions

- Skills are instructions for an AI agent, not documentation for humans. Write imperatively.
- Each skill should produce a specific deliverable (verdict table, assumption map, etc.) — name it explicitly.
- Processes should have clear phase boundaries where one step's output feeds the next.
- "Common Mistakes" should describe failure modes specific to this skill, not generic advice.
- Assumptions, findings, and assessments must be falsifiable/specific — never vague.

## Current Skills

- **hegelian-review** — Two-pass adversarial review (critic + steelman defender) producing a calibrated verdict table
- **double-loop-learning** — Surfaces hidden assumptions behind decisions, producing an assessed assumption map
