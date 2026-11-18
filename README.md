# skills-common

<p align="center"><em>Shared skills that are reusable across workflows. Keep them lean and general.</em></p>

<p align="center">
  <img alt="License MIT" src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge">
  <img alt="Agent Skills Standard" src="https://img.shields.io/badge/Agent%20Skills-Standard-6DA544?style=for-the-badge">
  <img alt="skills.sh Compatible" src="https://img.shields.io/badge/skills.sh-Compatible-1E6FFF?style=for-the-badge">
  <img alt="Runtime" src="https://img.shields.io/badge/Runtime-Claude%20Code%20·%20Codex%20·%20Cursor-8A2BE2?style=for-the-badge">
</p>

<p align="center"><strong>This repository contains reusable skills that are not specific to one workflow.</strong></p>

English | [中文](README.zh-CN.md)

* * *

## Install

### Project scope

Install into the current repo.

```bash
npx skills@latest add YangZhaoWeblog/skills-common -y
```

### Global scope

Install into your user space.

```bash
npx skills@latest add YangZhaoWeblog/skills-common -g -y
```

Project scope is the default. `-g` switches to user-level installation.

### Single skill

Install only one skill from this repository.

```bash
npx skills@latest add YangZhaoWeblog/skills-common --skill td-logic-writer -y
```

Install one local skill directory.

```bash
npx skills@latest add /Users/yangzhao/Code/skills-common/skills/shared/td-logic-writer -y
```

Use one skill without installing it.

```bash
npx skills@latest use YangZhaoWeblog/skills-common@td-logic-writer
```

Replace `td-logic-writer` with the target skill name. Add `-g` to install that single skill globally.

* * *

## Skills

| Skill | What it does |
| --- | --- |
| [td-challenge](skills/shared/td-challenge/SKILL.md) | Test an existing judgment or plan against the strongest objection and the evidence that could change it. |
| [td-cross-domain](skills/shared/td-cross-domain/SKILL.md) | Compare approaches from different fields and choose the best fit for the current problem. |
| [td-first-principles](skills/shared/td-first-principles/SKILL.md) | Trace a situation to reliable fundamentals before setting goals or choosing methods. |
| [td-logic-writer](skills/shared/td-logic-writer/SKILL.md) | Write concise judgment-system articles from messy notes. |
| [td-logic-writing-flow](skills/shared/td-logic-writing-flow/SKILL.md) | Route Obsidian writing tasks and enforce review gates. |
| [td-progress](skills/shared/td-progress/SKILL.md) | Review task progress and track milestones. |
| [td-wrong-way](skills/shared/td-wrong-way/SKILL.md) | Flag when a question, judgment, or action misses what matters, and reframe the problem when needed. |
| [tech-doc-writer](skills/shared/tech-doc-writer/SKILL.md) | Draft technical docs with a structured pipeline. |
| [td-external-agent](skills/shared/td-external-agent/README.md) | Delegate tasks to Codex, Claude Code, CodeBuddy or DSH CLI. |

## Layout

**skills/shared/** contains maintained skills. **skills-common** covers shared capabilities, [skills-develop](../skills-develop/README.md) covers development workflows, and [skills-learning](../skills-learning/README.md) covers learning workflows.
