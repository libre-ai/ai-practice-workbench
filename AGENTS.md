# ai-practice-workbench Canonical Agent Rules

> **Archived.** This repository is read-only once archived; its scope moved
> to https://github.com/libre-ai/personal-knowledge-workspace. Do not open
> new work here; propose it there.

## Purpose

Reserved couche-1 product home for Libre AI Practice Workbench: learn through
practice with AI while understanding the sources used and the work done by
the learner.
Doctrine lives upstream: https://raw.githubusercontent.com/libre-ai/project-governance/HEAD/AGENTS.md

## Domain doctrine

- The learner's own work stays distinguishable from AI-generated suggestions.
- No hidden scoring, and no scoring for human-resources decisions.
- `project.v1.yaml` is the authority on project state and admission
  criteria; the README "Project status" section is generated from it —
  never edit that section by hand.
- Recovered code (`apps/practices`) is not product qualification.
- Contract shapes are canonical in `libre-ai/schemas-and-contracts`, consumed
  pinned, never redefined here.

## Commands

- Prepare the pinned composition (target `ai-practice-workbench`):
  https://raw.githubusercontent.com/libre-ai/project-governance/HEAD/docs/LOCAL-COMPOSITION.md
- `bun run check` from this repository's root in the composition.
- Browser suite: `bun run --cwd apps/practices test:e2e --workers=1`.

## Working here

- Security > quality > performance > completeness, in that order on conflict.
- Check real state before editing: `git status --short` and the check above;
  never hide a red test.
- English for code, comments and this file.
- Never commit a machine-local absolute filesystem path, a secret or a
  personal identifier.
